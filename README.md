# speech-lipsync

This is an implementation of Web-Based Live Speech-Driven Lip-Sync (https://repositori.upf.edu/bitstream/handle/10230/28139/llorach_VSG16_web.pdf) for VR avatars. This involves capturing speaker stream of desired browser tab using Chrome extension and passing stream id to application and then do audio processing as mentioned by author in paper. As mentioned by author in paper, this solution is speaker dependent. We used Amazon Poly for Indian voice, In similar fashion one can use some other speaker and fine tune acoordingly for their solution.   

In order to make it work one has to deploy extension code either locally or on chrome webstore. Once one get the extension id, please update the same in getScreenId.html and also mention your domain in getScreenId.js.It will help to capture audio from your domain.Once Audio is captured stream is passed to application for processing using webRTC and WebAudio. Audio processing implementtaion is same as mentioned in paper. Thanks to Gerard Llorach for writing this paper. 
