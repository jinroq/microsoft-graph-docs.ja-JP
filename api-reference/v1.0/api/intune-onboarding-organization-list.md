---
title: organizations のリスト
description: organization オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6fb4fe8c27695e037320ef92f69c4a0b3809f512
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870932"
---
# <a name="list-organizations"></a><span data-ttu-id="4d0a2-103">organizations のリスト</span><span class="sxs-lookup"><span data-stu-id="4d0a2-103">List organizations</span></span>

> <span data-ttu-id="4d0a2-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4d0a2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d0a2-105">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="4d0a2-105">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4d0a2-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="4d0a2-106">Prerequisites</span></span>
<span data-ttu-id="4d0a2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d0a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d0a2-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4d0a2-109">Permission type</span></span>|<span data-ttu-id="4d0a2-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4d0a2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d0a2-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4d0a2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4d0a2-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d0a2-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="4d0a2-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4d0a2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d0a2-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d0a2-114">Not supported.</span></span>|
|<span data-ttu-id="4d0a2-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4d0a2-115">Application</span></span>|<span data-ttu-id="4d0a2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d0a2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d0a2-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4d0a2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization
```

## <a name="request-headers"></a><span data-ttu-id="4d0a2-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4d0a2-118">Request headers</span></span>
|<span data-ttu-id="4d0a2-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4d0a2-119">Header</span></span>|<span data-ttu-id="4d0a2-120">値</span><span class="sxs-lookup"><span data-stu-id="4d0a2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d0a2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d0a2-121">Authorization</span></span>|<span data-ttu-id="4d0a2-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4d0a2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d0a2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4d0a2-123">Accept</span></span>|<span data-ttu-id="4d0a2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4d0a2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d0a2-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="4d0a2-125">Request body</span></span>
<span data-ttu-id="4d0a2-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4d0a2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d0a2-127">応答</span><span class="sxs-lookup"><span data-stu-id="4d0a2-127">Response</span></span>
<span data-ttu-id="4d0a2-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [organization](../resources/intune-onboarding-organization.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="4d0a2-128">If successful, this method returns a `200 OK` response code and a collection of [organization](../resources/intune-onboarding-organization.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d0a2-129">例</span><span class="sxs-lookup"><span data-stu-id="4d0a2-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="4d0a2-130">要求</span><span class="sxs-lookup"><span data-stu-id="4d0a2-130">Request</span></span>
<span data-ttu-id="4d0a2-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4d0a2-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/organization
```

### <a name="response"></a><span data-ttu-id="4d0a2-132">応答</span><span class="sxs-lookup"><span data-stu-id="4d0a2-132">Response</span></span>
<span data-ttu-id="4d0a2-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4d0a2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



