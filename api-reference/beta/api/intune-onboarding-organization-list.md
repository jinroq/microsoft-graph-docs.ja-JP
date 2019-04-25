---
title: organizations のリスト
description: organization オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 067489dad7e08053cd4e6004f1e8b20fca479853
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32528506"
---
# <a name="list-organizations"></a><span data-ttu-id="ec3cd-103">organizations のリスト</span><span class="sxs-lookup"><span data-stu-id="ec3cd-103">List organizations</span></span>

> <span data-ttu-id="ec3cd-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ec3cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec3cd-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ec3cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec3cd-106">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ec3cd-106">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec3cd-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ec3cd-107">Prerequisites</span></span>
<span data-ttu-id="ec3cd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ec3cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec3cd-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ec3cd-110">Permission type</span></span>|<span data-ttu-id="ec3cd-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ec3cd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec3cd-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ec3cd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ec3cd-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec3cd-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ec3cd-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ec3cd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec3cd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ec3cd-115">Not supported.</span></span>|
|<span data-ttu-id="ec3cd-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ec3cd-116">Application</span></span>|<span data-ttu-id="ec3cd-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ec3cd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec3cd-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ec3cd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization
```

## <a name="request-headers"></a><span data-ttu-id="ec3cd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ec3cd-119">Request headers</span></span>
|<span data-ttu-id="ec3cd-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ec3cd-120">Header</span></span>|<span data-ttu-id="ec3cd-121">値</span><span class="sxs-lookup"><span data-stu-id="ec3cd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec3cd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec3cd-122">Authorization</span></span>|<span data-ttu-id="ec3cd-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ec3cd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec3cd-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ec3cd-124">Accept</span></span>|<span data-ttu-id="ec3cd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ec3cd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec3cd-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ec3cd-126">Request body</span></span>
<span data-ttu-id="ec3cd-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ec3cd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec3cd-128">応答</span><span class="sxs-lookup"><span data-stu-id="ec3cd-128">Response</span></span>
<span data-ttu-id="ec3cd-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [organization](../resources/intune-onboarding-organization.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ec3cd-129">If successful, this method returns a `200 OK` response code and a collection of [organization](../resources/intune-onboarding-organization.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec3cd-130">例</span><span class="sxs-lookup"><span data-stu-id="ec3cd-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec3cd-131">要求</span><span class="sxs-lookup"><span data-stu-id="ec3cd-131">Request</span></span>
<span data-ttu-id="ec3cd-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ec3cd-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/organization
```

### <a name="response"></a><span data-ttu-id="ec3cd-133">応答</span><span class="sxs-lookup"><span data-stu-id="ec3cd-133">Response</span></span>
<span data-ttu-id="ec3cd-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ec3cd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 622

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.organization",
      "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
      "mobileDeviceManagementAuthority": "intune",
      "certificateConnectorSetting": {
        "@odata.type": "microsoft.graph.certificateConnectorSetting",
        "status": 6,
        "certExpiryTime": "2017-01-01T00:00:03.9979674-08:00",
        "enrollmentError": "Enrollment Error value",
        "lastConnectorConnectionTime": "2017-01-01T00:02:50.2393584-08:00",
        "connectorVersion": "Connector Version value",
        "lastUploadVersion": 1
      }
    }
  ]
}
```





