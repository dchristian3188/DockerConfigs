FROM microsoft/windowsservercore
MAINTAINER dchristian3188

RUN powershell -NoProfile -Command \
    Install-PackageProvider -Name Nuget -Force -Verbose; \
    Install-Module -verbose -Force -Name xPSDesiredStateConfiguration;
