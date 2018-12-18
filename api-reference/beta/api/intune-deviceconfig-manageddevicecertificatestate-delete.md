---
title: ManagedDeviceCertificateState を削除します。
description: ManagedDeviceCertificateState を削除します。
author: tfitzmac
ms.openlocfilehash: e97757843bc8c4ef7444bd81cee6ffb0666ab94f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341616"
---
# <a name="delete-manageddevicecertificatestate"></a><span data-ttu-id="435ff-103">ManagedDeviceCertificateState を削除します。</span><span class="sxs-lookup"><span data-stu-id="435ff-103">Delete managedDeviceCertificateState</span></span>

> <span data-ttu-id="435ff-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="435ff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="435ff-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="435ff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="435ff-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="435ff-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="435ff-107">の[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="435ff-107">Deletes a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="435ff-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="435ff-108">Prerequisites</span></span>
<span data-ttu-id="435ff-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="435ff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="435ff-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="435ff-111">Permission type</span></span>|<span data-ttu-id="435ff-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="435ff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="435ff-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="435ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="435ff-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="435ff-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="435ff-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="435ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="435ff-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="435ff-116">Not supported.</span></span>|
|<span data-ttu-id="435ff-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="435ff-117">Application</span></span>|<span data-ttu-id="435ff-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="435ff-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="435ff-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="435ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="435ff-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="435ff-120">Request headers</span></span>
|<span data-ttu-id="435ff-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="435ff-121">Header</span></span>|<span data-ttu-id="435ff-122">値</span><span class="sxs-lookup"><span data-stu-id="435ff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="435ff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="435ff-123">Authorization</span></span>|<span data-ttu-id="435ff-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="435ff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="435ff-125">Accept</span><span class="sxs-lookup"><span data-stu-id="435ff-125">Accept</span></span>|<span data-ttu-id="435ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="435ff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="435ff-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="435ff-127">Request body</span></span>
<span data-ttu-id="435ff-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="435ff-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="435ff-129">応答</span><span class="sxs-lookup"><span data-stu-id="435ff-129">Response</span></span>
<span data-ttu-id="435ff-130">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="435ff-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="435ff-131">例</span><span class="sxs-lookup"><span data-stu-id="435ff-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="435ff-132">要求</span><span class="sxs-lookup"><span data-stu-id="435ff-132">Request</span></span>
<span data-ttu-id="435ff-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="435ff-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="435ff-134">応答</span><span class="sxs-lookup"><span data-stu-id="435ff-134">Response</span></span>
<span data-ttu-id="435ff-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="435ff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





