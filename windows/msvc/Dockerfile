FROM mcr.microsoft.com/windows/servercore:20H2

ENV chocolateyUseWindowsCompression false

RUN powershell -Command iex ((new-object net.webclient).DownloadString('https://chocolatey.org/install.ps1'));

RUN choco feature disable --name showDownloadProgress

RUN choco install python -y
RUN choco install python3 -y
RUN choco install visualstudio2022community -y
RUN choco install llvm -y
RUN choco install git -y
RUN choco install cmake -y
RUN choco install conan -y
RUN choco install ccache -y
RUN choco install cppcheck -y
RUN choco install opencppcoverage -y
RUN choco install go-task -y

CMD ["powershell"]
