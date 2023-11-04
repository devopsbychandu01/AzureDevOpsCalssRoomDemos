dotnet new sln -o HelloworldApp

cd HelloworldApp

dotnet new mvc -n HelloWorldApp.Web

dotnet sln .\HelloworldApp.sln add .\HelloWorldApp.Web\HelloWorldApp.Web.csproj

dotnet restore

dotnet build --no-restore --configuration release

# the output of the build will be present in HellowroldApp/HelloWorlApp.Web/bin/RElease/net7.0/*.dll

## launch application
dotnet <*.dll>

## you have to run this from the home folder you will get the proper web app

cd HelloWorldApp.Web

dotnet .\bin\Release\net7.0\HelloWorldApp.Web.dll

## change some information on the index.cshtml file.

# go to View/Home and edit file index.cshtml

#welcome to azure devops ci/cd

dotnet publish --no-build --configuration release

# the output will be published in the following directory.
.\HelloworldApp\HelloWorldApp.Web\bin\release\net7.0\publish\

# The publish code has to move to the web server.

# Install gitignore extention.
# fn + f1 --> add gitignore --> visualstudio --> append

