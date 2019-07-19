---
title: ManagedDeviceCertificateState の削除
description: ManagedDeviceCertificateState を削除します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc81e8ec2e8a1f2190f3ab9cc34a2753907e9652
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963010"
---
# <a name="delete-manageddevicecertificatestate"></a><span data-ttu-id="b6eea-103">ManagedDeviceCertificateState の削除</span><span class="sxs-lookup"><span data-stu-id="b6eea-103">Delete managedDeviceCertificateState</span></span>

> <span data-ttu-id="b6eea-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6eea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6eea-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b6eea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6eea-106">[ManagedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="b6eea-106">Deletes a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6eea-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="b6eea-107">Prerequisites</span></span>
<span data-ttu-id="b6eea-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b6eea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6eea-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b6eea-110">Permission type</span></span>|<span data-ttu-id="b6eea-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b6eea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6eea-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b6eea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b6eea-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6eea-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b6eea-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b6eea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6eea-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6eea-115">Not supported.</span></span>|
|<span data-ttu-id="b6eea-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b6eea-116">Application</span></span>|<span data-ttu-id="b6eea-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6eea-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6eea-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b6eea-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b6eea-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6eea-119">Request headers</span></span>
|<span data-ttu-id="b6eea-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6eea-120">Header</span></span>|<span data-ttu-id="b6eea-121">値</span><span class="sxs-lookup"><span data-stu-id="b6eea-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6eea-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6eea-122">Authorization</span></span>|<span data-ttu-id="b6eea-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="b6eea-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6eea-124">承諾</span><span class="sxs-lookup"><span data-stu-id="b6eea-124">Accept</span></span>|<span data-ttu-id="b6eea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b6eea-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6eea-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b6eea-126">Request body</span></span>
<span data-ttu-id="b6eea-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b6eea-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6eea-128">応答</span><span class="sxs-lookup"><span data-stu-id="b6eea-128">Response</span></span>
<span data-ttu-id="b6eea-129">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="b6eea-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b6eea-130">例</span><span class="sxs-lookup"><span data-stu-id="b6eea-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6eea-131">要求</span><span class="sxs-lookup"><span data-stu-id="b6eea-131">Request</span></span>
<span data-ttu-id="b6eea-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b6eea-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="b6eea-133">応答</span><span class="sxs-lookup"><span data-stu-id="b6eea-133">Response</span></span>
<span data-ttu-id="b6eea-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b6eea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





