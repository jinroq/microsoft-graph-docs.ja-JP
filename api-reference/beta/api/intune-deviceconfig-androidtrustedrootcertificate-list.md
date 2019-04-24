---
title: リスト androidtrustedrootcertificates
description: androidtrustedrootcertificate オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bb8ae6cfcb0072ceb4544c953c9f247686df361c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32475530"
---
# <a name="list-androidtrustedrootcertificates"></a><span data-ttu-id="89174-103">リスト androidtrustedrootcertificates</span><span class="sxs-lookup"><span data-stu-id="89174-103">List androidTrustedRootCertificates</span></span>

> <span data-ttu-id="89174-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89174-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89174-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="89174-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89174-106">[androidtrustedrootcertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="89174-106">List properties and relationships of the [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89174-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="89174-107">Prerequisites</span></span>
<span data-ttu-id="89174-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="89174-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89174-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="89174-110">Permission type</span></span>|<span data-ttu-id="89174-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="89174-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89174-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="89174-112">Delegated (work or school account)</span></span>|<span data-ttu-id="89174-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="89174-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="89174-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="89174-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89174-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89174-115">Not supported.</span></span>|
|<span data-ttu-id="89174-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="89174-116">Application</span></span>|<span data-ttu-id="89174-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89174-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89174-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="89174-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="89174-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="89174-119">Request headers</span></span>
|<span data-ttu-id="89174-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="89174-120">Header</span></span>|<span data-ttu-id="89174-121">値</span><span class="sxs-lookup"><span data-stu-id="89174-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89174-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="89174-122">Authorization</span></span>|<span data-ttu-id="89174-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="89174-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89174-124">承諾</span><span class="sxs-lookup"><span data-stu-id="89174-124">Accept</span></span>|<span data-ttu-id="89174-125">application/json</span><span class="sxs-lookup"><span data-stu-id="89174-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89174-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="89174-126">Request body</span></span>
<span data-ttu-id="89174-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="89174-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89174-128">応答</span><span class="sxs-lookup"><span data-stu-id="89174-128">Response</span></span>
<span data-ttu-id="89174-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[androidtrustedrootcertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="89174-129">If successful, this method returns a `200 OK` response code and a collection of [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89174-130">例</span><span class="sxs-lookup"><span data-stu-id="89174-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="89174-131">要求</span><span class="sxs-lookup"><span data-stu-id="89174-131">Request</span></span>
<span data-ttu-id="89174-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="89174-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="89174-133">応答</span><span class="sxs-lookup"><span data-stu-id="89174-133">Response</span></span>
<span data-ttu-id="89174-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="89174-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 624

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidTrustedRootCertificate",
      "id": "7f8d751e-751e-7f8d-1e75-8d7f1e758d7f",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
      "certFileName": "Cert File Name value"
    }
  ]
}
```





