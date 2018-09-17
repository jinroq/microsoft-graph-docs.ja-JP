# <a name="managementagenttype-enum-type"></a>managementAgentType 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

管理エージェントの種類です。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|EAS|1|デバイスは、Exchange サーバーによって管理されます。|
|mdm|2|デバイスは Intune MDM によって管理されます。|
|easMdm|3|デバイスは、Exchange サーバーによって管理されます。|
|intuneClient|4|Intune クライアントが管理されています。|
|easIntuneClient|5|デバイスは EAS と Intune クライアントによりデュアル管理されています。|
|configurationManagerClient|8|デバイスは構成マネージャによって管理されます。|
|configurationManagerClientMdm|10|デバイスは構成マネージャと MDM によって管理されます。|
|configurationManagerClientMdmEas|11|デバイスはは構成マネージャ、MDM および Eas によって管理されます。|
|不明|16|不明な管理エージェントの種類です。|
|jamf|32|デバイス属性は、Jamf からフェッチされます。|
|googleCloudDevicePolicyController|64|デバイスは、Google の CloudDPC によって管理されます。|








