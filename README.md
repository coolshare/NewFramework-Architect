New Framework: Architecture
=================================

By Mark Qian 8/2018 (markqian@hotmail.com)

<b>A. Introduction:</b><br/>
About a years ago, I started an UI of SDN (Software-defined networking) project from scrach. The requirements including the following:<br/>
<ul>
  <li>highly componentized: there is a protential to eventually deliver a platform where third-party coders can share the components used by company's primary UI</li>
  <li>rapidly changable: in many cases, PM want to sit with UI to apply design (modification or creation on the fly while discussing.</li>
  <li>model driven: server side will generate/deliver (even runtime) a list of "models" and UI should be able to  render them</li>
  <li>other "regular" requirments: highly dynamically (heavily streaming), highly graphicall (a variety of charts and operatable diagrams) and so on

</ul>
<b>B. Result:</b><br/> 
Currently, as a result, a framework has been established and several applications are built on the framework. The framework provides the following:<br/>
<ul>
  <li>highly componentized: any application, as a container, built on the framework contains two types of highly decoupled "objects": UI component (boxes in light blue below) and services (circles in orange). Pub/Sub is used for communication:</li>
  <img src="https://github.com/coolshare/NewFramework-Architect/blob/master/workflow3.png"/>
  As you can see in the diagram above, no object reference to others: for example, an UI component has no idea about whom its request (publish) is served by and a service also has no idea about where the request is coming and where the response from server is return to: "objects" in the container is hightly isolated!
  <li>rapidly changable: we only need about 5 minutes to put together a regular form or table and it takes only seconds to add/remove/modify a field since we only need to edit the UI schema and the rest will be taken care by the framework. You will see how in the <a href="https://github.com/coolshare/NewFramework-SchemaDriven" target="_blank">"Schema Driven"</a> section</li>
  <li>model driven: the framework can render any "regular" models out of model definition delivered by server. The rest of screens need some special "UI muscle". The percentage depends on application.</li>
  <li>One major character of this framework is that any application built on it contains no application logic (work flow) until the runtime - the application logic is loaded from a json configuration file at runtime. That is, the logic is extracted out of codes as data. The details are available in the <a href="https://github.com/coolshare/NewFramework-SchemaDriven" target="_blank">"Schema Driven"</a> section</li>
</ul>

<b>C. Details on Design and Implementation:</b><br/>
<ul>
  <li>1. Problem:</li>
  <li>2. Solution:</li>
</ul>

(Under construction)
