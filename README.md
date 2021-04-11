# GitHubUnityBuild

Demonstrates how to get GitHub Actions to compile Unity projects

1. Fork this project
2. Add unity key using Settings > Secrets > New Repository Secret.
    - UNITY_LICENSE: ....
    - You can use the license in personal-license-unity.txt OR follow the instructions at https://game.ci/docs/github/activation

3. Add/Modify files in /src directory
4. Every time changes are pushed to the repository, a new WebGL build will be created. Download the WebGL build from Actions > Unity Build Actions under "Artifacts" at the bottom
5. See .github/workflows/unitybuilder.yml for the actions used to build the WebGL. It can also be used to build Windows executables and other standalone executables.
