Welcome to a Barclamp for the Crowbar Framework project
=======================================================
_Copyright 2011, Dell, Inc._

The code and documentation is distributed under the Apache 2 license (http://www.apache.org/licenses/LICENSE-2.0.html). Contributions back to the source are encouraged.

The Crowbar Framework (https://github.com/dellcloudedge/crowbar) was developed by the Dell CloudEdge Solutions Team (http://dell.com/openstack) as a OpenStack installer (http://OpenStack.org) but has evolved as a much broader function tool. 
A Barclamp is a module component that implements functionality for Crowbar.  Core barclamps operate the essential functions of the Crowbar deployment mechanics while other barclamps extend the system for specific applications.

* This functonality of this barclamp DOES NOT stand alone, the Crowbar Framework is required * 

About this Barclamp-keystone
-------------------------------------

Information for this barclamp is maintained on the Crowbar Framework Wiki: https://github.com/dellcloudedge/crowbar/wiki

This is based on OpenStack.org distribution

This barclamp is designed to be used in conjunction with the OpenStack High-Availability barclamps please review the https://github.com/crowbar/barclamp-openstack-titanium-loadbalancer for deployment information.

This barclamp should be applued to  3 controller nodes.

Compute barclamp is responsible for installing and configuring Openstack nova on the controller and compute nodes. The compute barclamp is a cloud computing fabric controller. Essentially the nova is the primary part of an infrastructure as a service system. Nova is responsible for providing computing resources and the ability to spawn virtual machines. Nova has the below componentry that manage various processes and functionality. Nova-compute service is installed on the compute nodes while the rest of the nova services are installed on the controller nodes. 

nova-api 
nova-scheduler 
nova-conductor 
nova-console 
nova-consoleauth 
nova-compute 

Prerequisite for the nova proposal are to be applied in the following HAProxy, Percona, RabbitMQ, Keystone, Glance, Cinder and Quantum. Nova proposal as usual needs to be created and saved with the correct settings. Hypervisor selection and node allocation for nova deployment must be set. 

Three controller nodes are added to the nova-multi-controller role and as many as compute nodes required can be added to the nova-multi-compute role.





Legals
-------------------------------------
Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

