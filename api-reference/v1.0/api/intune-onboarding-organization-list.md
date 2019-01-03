---
title: organizations のリスト
description: organization オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
ms.openlocfilehash: 4ad5c23d038274de62a7ab4f4e9c0a467918e754
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309066"
---
# <a name="list-organizations"></a><span data-ttu-id="8b19f-103">organizations のリスト</span><span class="sxs-lookup"><span data-stu-id="8b19f-103">List organizations</span></span>

> <span data-ttu-id="8b19f-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8b19f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8b19f-105">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="8b19f-105">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8b19f-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="8b19f-106">Prerequisites</span></span>
<span data-ttu-id="8b19f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8b19f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b19f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8b19f-109">Permission type</span></span>|<span data-ttu-id="8b19f-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8b19f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b19f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8b19f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8b19f-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b19f-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="8b19f-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8b19f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b19f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b19f-114">Not supported.</span></span>|
|<span data-ttu-id="8b19f-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8b19f-115">Application</span></span>|<span data-ttu-id="8b19f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b19f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b19f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8b19f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization
```

## <a name="request-headers"></a><span data-ttu-id="8b19f-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8b19f-118">Request headers</span></span>
|<span data-ttu-id="8b19f-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8b19f-119">Header</span></span>|<span data-ttu-id="8b19f-120">値</span><span class="sxs-lookup"><span data-stu-id="8b19f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b19f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b19f-121">Authorization</span></span>|<span data-ttu-id="8b19f-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8b19f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b19f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8b19f-123">Accept</span></span>|<span data-ttu-id="8b19f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8b19f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b19f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="8b19f-125">Request body</span></span>
<span data-ttu-id="8b19f-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8b19f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b19f-127">応答</span><span class="sxs-lookup"><span data-stu-id="8b19f-127">Response</span></span>
<span data-ttu-id="8b19f-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [organization](../resources/intune-onboarding-organization.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="8b19f-128">If successful, this method returns a `200 OK` response code and a collection of [organization](../resources/intune-onboarding-organization.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b19f-129">例</span><span class="sxs-lookup"><span data-stu-id="8b19f-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="8b19f-130">要求</span><span class="sxs-lookup"><span data-stu-id="8b19f-130">Request</span></span>
<span data-ttu-id="8b19f-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8b19f-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/organization
```

### <a name="response"></a><span data-ttu-id="8b19f-132">応答</span><span class="sxs-lookup"><span data-stu-id="8b19f-132">Response</span></span>
<span data-ttu-id="8b19f-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8b19f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 196

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.organization",
      "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
      "mobileDeviceManagementAuthority": "intune"
    }
  ]
}
```


