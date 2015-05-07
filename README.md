# feedback-to-gitlab

Webserver to generate Gitlab issues for user feedback generated by [ivoviz/feedback](https://github.com/ivoviz/feedback)

## Install

    npm install feedback-to-gitlab

You have to adapt your settings and credentials:

    cp config.json.example config.json
    edit config.json

On the website where you want to gain user feedback you have to include [ivoviz/feedback](https://github.com/ivoviz/feedback). Example configuration:

    jQuery.feedback({
      ajaxURL: 'http://localhost',
      html2canvasURL: 'html2canvas.min.js',
      requireContactInfo: true
    })

This module has been developed for the fork [yq314/feedback](https://github.com/yq314/feedback) which adds an additional contact form field, but it should work for the original feedback library too.

## Usage

    npm start

## Generated Issue

![Screenshot](screenshot.png)