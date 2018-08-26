New Framework: Architecture
=================================

By Mark Qian 8/2018 (markqian@hotmail.com)

<b>A. Introduction:</b><br/>
About a years ago, I started an UI of SDN (Software-defined networking) project from scrach. The requirements including the following:<br/>
<ul>
  <li>highly componentized: there is a protential to eventually deliver a platform where third-party coders can share the components used by company's primary UI</li>
  <li>rapidly changable: in many cases, PM want to sit with UI to apply design (modification or creation on the fly while discussing.</li>
  <li>model driven: server side will generate/deliver (even runtime) a list of "models" and UI should be able to  render them</li>
  <li>there could be a mobile interface</li>
</ul>
<b>B. Result:</b><br/> 
Currently, as a result, a framework has been established and several applications are built on the framework. The framework provides the following:<br/>
<ul>
  <li>highly componentized: any application, as a container, built on the framework contains two types of highly decoupled "objects": UI component (boxes in light blue below) and services (circles in orange). Pub/sub is used for communication:</li>
  <img src="https://github.com/coolshare/NewFramework-Architect/blob/master/workflow3.png"/>
  As you can see, no object reference to others: for example, an UI component has no idea about whom its request (publish) is served by and a service also has no idea about where the request is coming and where the response from server is return to: "objects" in the container is hightly isolated!
  <li>rapidly changable: in many cases, PM want to sit with UI to apply design (modification or creation on the fly while discussing.</li>
  <li>model driven: server side will generate/deliver (even runtime) a list of "models" and UI should be able to  render them</li>
  <li>there could be a mobile interface</li>
</ul>

I started this project using React backed by Redux but I eventually completely remove Redux from my application and used my own architecture.
The result in the architecture aspect is that 
There are several reasons for not using Redux

<b>B. Problem:</b><br/>

<b>C. Solution:</b><br/>

