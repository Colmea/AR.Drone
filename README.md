## AR.Drone [![Build Status](https://travis-ci.org/Ruslan-B/AR.Drone.png)](https://travis-ci.org/Ruslan-B/AR.Drone)

The AR.Drone 2.0 controlling library for C#/.NET and Mono, with video support.  
Built over the original [AR.Drone SDK](https://projects.ardrone.org) 2.0.1 - using lastest drone firmware.

If case you are looking for Windows RT/Windows Phone support please check this project [ARDrone2Windows](https://github.com/ARDrone2Windows/SDK).

## Dependencies

[FFmpeg.AutoGen](https://github.com/Ruslan-B/FFmpeg.AutoGen) - .NET wrapper for FFmpeg.  

## Status

All major features are supported - video, configuration and control.  
This library is still under heavy development, 
so please don't be suprised if you find some functionality missing or undocumented.  

## Build

How to build from scratch:  
- Clone this:

```bash
git clone git://github.com/Ruslan-B/AR.Drone.git   
cd AR.Drone   
git submodule update --init   
```  

- For the video support please review: *[Usage](https://github.com/Ruslan-B/FFmpeg.AutoGen#Usage)* section of the [FFmpeg.AutoGen](https://github.com/Ruslan-B/FFmpeg.AutoGen) project.

- Build AR.Drone solution with MonoDevelop, VS2010 or VS2012.

## Kinect Usage

The solution includes WPF application - AR.Drone.Kinect, wich let you control your AR Drone with your Kinect.
Plug your Kinect before run application. Then wait for speech synthetizer initialization.

/!\ *Stay far away from AR Drone when running application, especially if you're inside. Otherwise, voice commands are not detected due to noise* /!\

### Kinect voice commands

To control your AR Drone with voice commands, say "DRONE" to enable voice command +before each command+ (protection for misunderstood words).

Here is a list of available commands:
- *"Take off"* : To enable drone and take off.
- *"Stop"* : To disable drone and land.


## Usage

The solution includes Winform application - AR.Drone.WinApp, it provides minimalistic interface 
for controling and displaying video from the AR.Drone 2.0.

##License

Copyright 2013 Ruslan Balanukhin ruslan.balanukhin@gmail.com

GNU Lesser General Public License (LGPL) version 3 or later.  
http://www.gnu.org/licenses/lgpl.html

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
