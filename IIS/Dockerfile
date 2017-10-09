FROM microsoft/iis

RUN mkdir C:\site

RUN powershell -NoProfile -Command \
    Import-module IISAdministration; \
    New-IISSite -Name "Site" -PhysicalPath C:\site -BindingInformation "*:8000:"; \
    Copy -Path C:\inetpub\wwwroot\*  -Destination C:\site\ -Recurse -Force -Verbose
EXPOSE 8000
