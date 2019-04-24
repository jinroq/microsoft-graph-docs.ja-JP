---
title: windows10EndpointProtectionConfigurations のリスト
description: windows10EndpointProtectionConfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 75e2797027aa87854b5946b336115fae61b43b5d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463118"
---
# <a name="list-windows10endpointprotectionconfigurations"></a><span data-ttu-id="74ae2-103">windows10EndpointProtectionConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="74ae2-103">List windows10EndpointProtectionConfigurations</span></span>

> <span data-ttu-id="74ae2-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="74ae2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74ae2-105">[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="74ae2-105">List properties and relationships of the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74ae2-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="74ae2-106">Prerequisites</span></span>
<span data-ttu-id="74ae2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74ae2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74ae2-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="74ae2-109">Permission type</span></span>|<span data-ttu-id="74ae2-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="74ae2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74ae2-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="74ae2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="74ae2-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="74ae2-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="74ae2-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="74ae2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74ae2-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74ae2-114">Not supported.</span></span>|
|<span data-ttu-id="74ae2-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="74ae2-115">Application</span></span>|<span data-ttu-id="74ae2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74ae2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74ae2-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="74ae2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="74ae2-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="74ae2-118">Request headers</span></span>
|<span data-ttu-id="74ae2-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="74ae2-119">Header</span></span>|<span data-ttu-id="74ae2-120">値</span><span class="sxs-lookup"><span data-stu-id="74ae2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74ae2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="74ae2-121">Authorization</span></span>|<span data-ttu-id="74ae2-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="74ae2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74ae2-123">承諾</span><span class="sxs-lookup"><span data-stu-id="74ae2-123">Accept</span></span>|<span data-ttu-id="74ae2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="74ae2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74ae2-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="74ae2-125">Request body</span></span>
<span data-ttu-id="74ae2-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="74ae2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74ae2-127">応答</span><span class="sxs-lookup"><span data-stu-id="74ae2-127">Response</span></span>
<span data-ttu-id="74ae2-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="74ae2-128">If successful, this method returns a `200 OK` response code and a collection of [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74ae2-129">例</span><span class="sxs-lookup"><span data-stu-id="74ae2-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="74ae2-130">要求</span><span class="sxs-lookup"><span data-stu-id="74ae2-130">Request</span></span>
<span data-ttu-id="74ae2-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="74ae2-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="74ae2-132">応答</span><span class="sxs-lookup"><span data-stu-id="74ae2-132">Response</span></span>
<span data-ttu-id="74ae2-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="74ae2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



