BUILD THE APK USING ONLY YOUR PHONE (CLOUD BUILD)

This project now includes a GitHub Actions workflow that builds a debug APK on GitHub's servers. You do not need Android Studio on your phone.

1. Download and extract AviatorAnalyzerAndroid.zip in your phone's file manager.
2. In your browser, sign in or create an account at https://github.com.
3. Create a NEW repository. Give it a name such as AviatorAnalyzerAndroid. For easiest setup, set it to Public (do not upload private or personal information).
4. Upload the CONTENTS of the extracted AviatorAnalyzerAndroid folder to the repository, not the ZIP itself. Make sure .github/workflows/build-apk.yml is included. Some mobile file pickers hide folders beginning with a dot; if you cannot upload .github, use GitHub's website to create the workflow file at .github/workflows/build-apk.yml and paste the contents from this project.
5. Commit the files to the main branch.
6. Open the repository's Actions tab, select "Build Android APK", tap "Run workflow", and run it.
7. Wait for the workflow to finish with a green check mark. Open that completed run and download the artifact named "AviatorAnalyzer-debug-apk". GitHub may download it as a ZIP.
8. Extract the artifact ZIP. Tap app-debug.apk to install it. If Android prompts you, allow your browser or file manager to install unknown apps, then return and tap Install.

Troubleshooting:
- If the build fails, open the failed workflow run and send a screenshot of the red error/log to ChatGPT.
- A debug APK is unsigned for Play Store distribution but can generally be installed manually on your own phone.
- The app analyzes historical results only. It cannot reliably predict future random multipliers.
- Do not publish account passwords, API keys, or personal documents in a repository.
