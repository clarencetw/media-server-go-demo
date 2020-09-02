你好！
很冒昧用这样的方式来和你沟通，如有打扰请忽略我的提交哈。我是光年实验室（gnlab.com）的HR，在招Golang开发工程师，我们是一个技术型团队，技术氛围非常好。全职和兼职都可以，不过最好是全职，工作地点杭州。
我们公司是做流量增长的，Golang负责开发SAAS平台的应用，我们做的很多应用是全新的，工作非常有挑战也很有意思，是国内很多大厂的顾问。
如果有兴趣的话加我微信：13515810775  ，也可以访问 https://gnlab.com/，联系客服转发给HR。
# media-server-go-demo


media server go demo  for  https://github.com/notedit/media-server-go



## Build 
#### Ubuntu 18.04.2 LTS
```shell
mkdir wk_webrtc && cd wk_webrtc
git clone --recurse-submodules https://github.com/notedit/media-server-go.git
git clone https://github.com/notedit/media-server-go-demo.git


# build media-server-go
cd ../media-server-go && make && go build 

# build media-server-go-demo
cd ../media-server-go-demo

# broadcast 
go build 

# recording
go build 

# rtmp-to-webrtc 
sudo apt-get install libgstreamer1.0-0 gstreamer1.0-plugins-base gstreamer1.0-libav gstreamer1.0-plugins-bad libgstreamer-plugins-bad1.0-dev 

go build

# rtp-streamer
the same with rtmp-to-webrtc 

# server-to-server 
go build 

# sfu
go build 

# video-mixer
go build 

# webrtc-to-hls
go build

# webrtc-to-rtmp
go build 

```

## Examples

- [WebRTC-Broadcast](https://github.com/notedit/media-server-go-demo/tree/master/broadcast): WebRTC publish and play 
- [WebRTC-Record](https://github.com/notedit/media-server-go-demo/tree/master/recording): WebRTC record
- [RTMP-To-WebRTC](https://github.com/notedit/media-server-go-demo/tree/master/rtmp-to-webrtc): Rtmp to webrtc
- [Server-To-Server](https://github.com/notedit/media-server-go-demo/tree/master/server-to-server): WebRTC server relay
- [WebRTC-To-RTMP](https://github.com/notedit/media-server-go-demo/tree/master/webrtc-to-rtmp): WebRTC to rtmp
- [WebRTC-To-HLS](https://github.com/notedit/media-server-go-demo/tree/master/webrtc-to-hls): WebRTC to hls
