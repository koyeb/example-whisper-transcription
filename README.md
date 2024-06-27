<div align="center">
  <a href="https://koyeb.com">
    <img src="https://www.koyeb.com/static/images/icons/koyeb.svg" alt="Logo" width="80" height="80">
  </a>
  <h3 align="center">Koyeb Serverless Platform</h3>
  <p align="center">
    Deploy a Whisper Transcription Service on Koyeb
    <br />
    <a href="https://koyeb.com">Learn more about Koyeb</a>
    ·
    <a href="https://koyeb.com/docs">Explore the documentation</a>
    ·
    <a href="https://koyeb.com/tutorials">Discover our tutorials</a>
  </p>
</div>


## About Koyeb and the Whisper transcription service example application

Koyeb is a developer-friendly serverless platform to deploy apps globally. No-ops, servers, or infrastructure management.

This repository is designed to show how to deploy a transcription service application, written in Python to Koyeb.  The application uses [Streamlit](https://streamlit.io/) to build and serve a simple web interface and [OpenAI Whisper](https://github.com/openai/whisper) to transcribe an audio file in real time.  The application runs on Koyeb's GPU instances for high performance and scalability.

## Getting Started

Follow the steps below to deploy the Whisper transcription service to your Koyeb account.

### Requirements

To use this repository, you need:

* A Koyeb account to build the `Dockerfile` and deploy it to the platform.  If you don't already have an account, you can [sign-up for free](https://app.koyeb.com/auth/signup).

### Deploy using the Koyeb button

The fastest way to deploy the Whisper transcription service is to click the **Deploy to Koyeb** button below.

[![Deploy to Koyeb](https://www.koyeb.com/static/images/deploy/button.svg)](https://app.koyeb.com/deploy?name=whisper-transcription&type=git&repository=koyeb%2Fexample-whisper-transcription&branch=main&builder=dockerfile&instance_type=gpu-nvidia-rtx-4000-sff-ada&env%5B%5D=&ports=8000%3Bhttp%3B%2F)

Clicking on this button brings you to the Koyeb App creation page with the settings pre-configured to launch this application.

_To modify this application example, you will need to fork this repository. Checkout the [fork and deploy](#fork-and-deploy-to-koyeb) instructions._

### Fork and deploy to Koyeb

If you want to customize and enhance this application, you need to fork this repository.

If you used the **Deploy to Koyeb** button, you can simply link your service to your forked repository to be able to push changes.  Alternatively, you can manually create the application as described below.

On the [Koyeb Control Panel](https://app.koyeb.com/), on the **Overview** tab, initiate the app creation and deployment process by clicking **Create Service** and then choosing **Create web service**.

1. Select **GitHub** as the deployment source.
2. Select your repository from the menu.
3. In the **Instance** selection, select a GPU Instance.
4. In the **Builder** section, choose **Dockerfile**.
5. Click **Deploy**.

The repository will be pulled, built, and deployed on Koyeb. Once the deployment is complete, it will be accessible using the Koyeb subdomain for your service.

## Contributing

If you have any questions, ideas or suggestions regarding this application sample, feel free to open an [issue](https://github.com/koyeb/example-whisper-transcription/issues) or fork this repository and open a [pull request](https://github.com/koyeb/example-whisper-transcription/pulls).

## Contact

[Koyeb](https://www.koyeb.com) - [@gokoyeb](https://twitter.com/gokoyeb) - [Slack](http://slack.koyeb.com/)
