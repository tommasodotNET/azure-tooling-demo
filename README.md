# Azure Tooling Demo

azd config set alpha.infraSynth on
azd infra synth --> show yaml and biceps

azd init

azd auth login
azd up

dotnet run --project AspireSample.AppHost/AspireSample.AppHost.csproj --publisher manifest --output-path ../aspire-manifest.json

dotnet add package Aspire.Hosting.Azure --version 8.0.0-preview.4.24156.9

var cache = builder.AddRedis("cache")
    .PublishAsAzureRedis();