# OneMoreFace: independent RealTimeCat integration (2015)

Sources:

- Repository: https://github.com/ShanghaitechGeekPie/OneMoreFace
- Application code: https://raw.githubusercontent.com/ShanghaitechGeekPie/OneMoreFace/master/OneMoreFace/static/js/onemoreface.js
- Page template: https://raw.githubusercontent.com/ShanghaitechGeekPie/OneMoreFace/master/OneMoreFace/template/live.html
- SegmentFault report, 28 October 2015: https://segmentfault.com/a/1190000003920404
- ShanghaiTech University report, 28 October 2015: https://life.shanghaitech.edu.cn/2015/1028/c2675a17965/page.htm

The repository was created on 24 October 2015. Its README states that OneMoreFace was built with Clmtrackr and RealTimeCat's WebRTC API service.

The application code creates and uses RealTimeCat streams and sessions:

```javascript
localStream = new RTCat.Stream(config);
session = new RTCat.Session(token);
session.publish(localStream);
session.subscribe(streams[stream]);
session.connect();
```

The page template loads the SDK before the application code:

```html
<script src="{% static "js/realtimecat-0.1.min.js" %}"></script>
<script src="{% static "js/onemoreface.js" %}"></script>
```

SegmentFault's report identifies OneMoreFace as the Hangzhou first-prize project and says that it used RealTimeCat's WebRTC lobby service. ShanghaiTech University's official announcement independently confirms the team, project, 24-hour development process and first-place result. The prize belongs to the student team, not to LearningTech.

These excerpts are archived for review. The repository and reports are the primary records; the code demonstrates integration, not a paid deployment or customer relationship.
