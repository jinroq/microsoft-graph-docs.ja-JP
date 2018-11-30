---
title: windows10EndpointProtectionConfigurations のリスト
description: windows10EndpointProtectionConfiguration オブジェクトのプロパティとリレーションシップをリストします。
ms.openlocfilehash: 3c656bd865ef3a6b631243c3637457d081150ccf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021592"
---
# <a name="list-windows10endpointprotectionconfigurations"></a><span data-ttu-id="c7371-103">windows10EndpointProtectionConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="c7371-103">List windows10EndpointProtectionConfigurations</span></span>

> <span data-ttu-id="c7371-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c7371-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7371-105">[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c7371-105">List properties and relationships of the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c7371-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="c7371-106">Prerequisites</span></span>
<span data-ttu-id="c7371-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c7371-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7371-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c7371-109">Permission type</span></span>|<span data-ttu-id="c7371-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c7371-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7371-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c7371-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c7371-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7371-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c7371-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c7371-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7371-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7371-114">Not supported.</span></span>|
|<span data-ttu-id="c7371-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c7371-115">Application</span></span>|<span data-ttu-id="c7371-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7371-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7371-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c7371-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c7371-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c7371-118">Request headers</span></span>
|<span data-ttu-id="c7371-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c7371-119">Header</span></span>|<span data-ttu-id="c7371-120">値</span><span class="sxs-lookup"><span data-stu-id="c7371-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7371-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7371-121">Authorization</span></span>|<span data-ttu-id="c7371-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c7371-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7371-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c7371-123">Accept</span></span>|<span data-ttu-id="c7371-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c7371-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7371-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c7371-125">Request body</span></span>
<span data-ttu-id="c7371-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c7371-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7371-127">応答</span><span class="sxs-lookup"><span data-stu-id="c7371-127">Response</span></span>
<span data-ttu-id="c7371-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="c7371-128">If successful, this method returns a `200 OK` response code and a collection of [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7371-129">例</span><span class="sxs-lookup"><span data-stu-id="c7371-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="c7371-130">要求</span><span class="sxs-lookup"><span data-stu-id="c7371-130">Request</span></span>
<span data-ttu-id="c7371-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c7371-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="c7371-132">応答</span><span class="sxs-lookup"><span data-stu-id="c7371-132">Response</span></span>
<span data-ttu-id="c7371-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c7371-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4834

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
      "id": "09709403-9403-0970-0394-700903947009",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "firewallBlockStatefulFTP": true,
      "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
      "firewallPreSharedKeyEncodingMethod": "none",
      "firewallIPSecExemptionsAllowNeighborDiscovery": true,
      "firewallIPSecExemptionsAllowICMP": true,
      "firewallIPSecExemptionsAllowRouterDiscovery": true,
      "firewallIPSecExemptionsAllowDHCP": true,
      "firewallCertificateRevocationListCheckMethod": "none",
      "firewallMergeKeyingModuleSettings": true,
      "firewallPacketQueueingMethod": "disabled",
      "firewallProfileDomain": {
        "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
        "firewallEnabled": "blocked",
        "stealthModeBlocked": true,
        "incomingTrafficBlocked": true,
        "unicastResponsesToMulticastBroadcastsBlocked": true,
        "inboundNotificationsBlocked": true,
        "authorizedApplicationRulesFromGroupPolicyMerged": true,
        "globalPortRulesFromGroupPolicyMerged": true,
        "connectionSecurityRulesFromGroupPolicyMerged": true,
        "outboundConnectionsBlocked": true,
        "inboundConnectionsBlocked": true,
        "securedPacketExemptionAllowed": true,
        "policyRulesFromGroupPolicyMerged": true
      },
      "firewallProfilePublic": {
        "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
        "firewallEnabled": "blocked",
        "stealthModeBlocked": true,
        "incomingTrafficBlocked": true,
        "unicastResponsesToMulticastBroadcastsBlocked": true,
        "inboundNotificationsBlocked": true,
        "authorizedApplicationRulesFromGroupPolicyMerged": true,
        "globalPortRulesFromGroupPolicyMerged": true,
        "connectionSecurityRulesFromGroupPolicyMerged": true,
        "outboundConnectionsBlocked": true,
        "inboundConnectionsBlocked": true,
        "securedPacketExemptionAllowed": true,
        "policyRulesFromGroupPolicyMerged": true
      },
      "firewallProfilePrivate": {
        "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
        "firewallEnabled": "blocked",
        "stealthModeBlocked": true,
        "incomingTrafficBlocked": true,
        "unicastResponsesToMulticastBroadcastsBlocked": true,
        "inboundNotificationsBlocked": true,
        "authorizedApplicationRulesFromGroupPolicyMerged": true,
        "globalPortRulesFromGroupPolicyMerged": true,
        "connectionSecurityRulesFromGroupPolicyMerged": true,
        "outboundConnectionsBlocked": true,
        "inboundConnectionsBlocked": true,
        "securedPacketExemptionAllowed": true,
        "policyRulesFromGroupPolicyMerged": true
      },
      "defenderAttackSurfaceReductionExcludedPaths": [
        "Defender Attack Surface Reduction Excluded Paths value"
      ],
      "defenderGuardedFoldersAllowedAppPaths": [
        "Defender Guarded Folders Allowed App Paths value"
      ],
      "defenderAdditionalGuardedFolders": [
        "Defender Additional Guarded Folders value"
      ],
      "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
      "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
      "defenderSecurityCenterBlockExploitProtectionOverride": true,
      "appLockerApplicationControl": "enforceComponentsAndStoreApps",
      "smartScreenEnableInShell": true,
      "smartScreenBlockOverrideForFiles": true,
      "applicationGuardEnabled": true,
      "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
      "applicationGuardBlockNonEnterpriseContent": true,
      "applicationGuardAllowPersistence": true,
      "applicationGuardForceAuditing": true,
      "applicationGuardBlockClipboardSharing": "blockBoth",
      "applicationGuardAllowPrintToPDF": true,
      "applicationGuardAllowPrintToXPS": true,
      "applicationGuardAllowPrintToLocalPrinters": true,
      "applicationGuardAllowPrintToNetworkPrinters": true,
      "bitLockerDisableWarningForOtherDiskEncryption": true,
      "bitLockerEnableStorageCardEncryptionOnMobile": true,
      "bitLockerEncryptDevice": true,
      "bitLockerRemovableDrivePolicy": {
        "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
        "encryptionMethod": "aesCbc256",
        "requireEncryptionForWriteAccess": true,
        "blockCrossOrganizationWriteAccess": true
      }
    }
  ]
}
```



