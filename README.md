ports:
  - port: 8001
tasks:
  - before: |
      export JAVA_HOME="/usr/lib/jvm/java-1.8.0-openjdk-amd64"
      export PATH=$JAVA_HOME/bin:$ANDROID_HOME/bin:$ANDROID_HOME/platform-tools:$PATH
      mkdir -p /home/gitpod/.android
      touch /home/gitpod/.android/repositories.cfg
    init: |
      echo "Instalando Cordova"
      npm install -g cordova
      echo "Instalando SDK"
      mkdir -p /workspace/android-sdk && cd /workspace/android-sdk && wget https://dl.google.com/android/repository/sdk-tools-linux-4333796.zip && unzip sdk-tools-linux-4333796.zip && rm -f sdk-tools-linux-4333796.zip
      /workspace/android-sdk/tools/bin/sdkmanager "platform-tools" "platforms;android-28" "build-tools;28.0.3" && /workspace/android-sdk/tools/bin/sdkmanager --lisences
image:
  file: .gitpod.Dockerfile
