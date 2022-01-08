# Pi-hole

> An Alfred workflow to control [Pi-hole](https://pi-hole.net/) quicky.

## Demonstration video

https://www.youtube.com/watch?v=Yr9M-OwujDk

## Usage

Use Alfred keyword `pihole` and choose one of the commands:

`Admin` to open the admin web interface.

`Disable` to disable Pi-hole.

`Enable` to enable Pi-hole.

`Status` to display enable/disable status.

You may also setup hotkeys as shortcuts to disable and enable Pi-hole.

## Setup workflow

Before you use this workflow you need to set it up. To do so, open the workflow configuration to set its [environment variables](https://www.alfredapp.com/help/workflows/advanced/variables/#environment).

### Mandatory variables

`url`
	Set the URL to the admin web-interface.
	*For example: http://192.168.1.1:8089/admin/*

`host_address`
	Set IP address or name of the host.
	*For example: 192.168.1.1*

`host_user`
	Set name of the host user.
	*For example: pi*

### Optional variables

`host_password` (optional)
	Set password of the host user,
	if you don't use [ssh key](https://en.wikipedia.org/wiki/Ssh-keygen).

`container` (optional)
	Set [docker](https://www.docker.com/) container name.
	*For example: pihole*

`disable_duration` (optional)
	Set duration for disable command until Pi-hole gets enabled automatically.
	*For example: 5m*
	Leave empty for infinite duration.

## External trigger

With Alfred 4.1 upwards you can use the external triggers of this workflow to use its actions from other workflows or Apple Scripts. (see: https://www.alfredapp.com/help/workflows/triggers/external/)

## Background of the idea

As I search for products to purchase, I sometimes like to click on advertised links intentionally, which is not possible, if Pi-hole is enabled. It's a bit annoying and slow to call the web admin interface, login and hit the disable button. To quickly control Pi-hole in this scenario, an Alfred workflow is a perfect solution and I created it.

## MIT License

Copyright 2022 Tamio Honma <tamio@honma.de>

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.