---
title: assign アクション
description: まだ文書化されていません
ms.openlocfilehash: 3bdc4f9e20f866f6617bd73ccb1d915b34523f13
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073224"
---
# <a name="assign-action"></a><span data-ttu-id="13025-103">assign アクション</span><span class="sxs-lookup"><span data-stu-id="13025-103">assign action</span></span>

> <span data-ttu-id="13025-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="13025-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13025-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13025-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="13025-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="13025-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="13025-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="13025-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="13025-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="13025-108">Prerequisites</span></span>
<span data-ttu-id="13025-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="13025-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13025-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="13025-111">Permission type</span></span>|<span data-ttu-id="13025-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="13025-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13025-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="13025-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13025-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13025-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="13025-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="13025-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13025-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13025-116">Not supported.</span></span>|
|<span data-ttu-id="13025-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="13025-117">Application</span></span>|<span data-ttu-id="13025-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13025-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13025-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="13025-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="13025-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13025-120">Request headers</span></span>
|<span data-ttu-id="13025-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13025-121">Header</span></span>|<span data-ttu-id="13025-122">値</span><span class="sxs-lookup"><span data-stu-id="13025-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13025-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="13025-123">Authorization</span></span>|<span data-ttu-id="13025-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="13025-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13025-125">Accept</span><span class="sxs-lookup"><span data-stu-id="13025-125">Accept</span></span>|<span data-ttu-id="13025-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13025-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13025-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="13025-127">Request body</span></span>
<span data-ttu-id="13025-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="13025-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="13025-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="13025-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="13025-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13025-130">Property</span></span>|<span data-ttu-id="13025-131">型</span><span class="sxs-lookup"><span data-stu-id="13025-131">Type</span></span>|<span data-ttu-id="13025-132">説明</span><span class="sxs-lookup"><span data-stu-id="13025-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13025-133">assignments</span><span class="sxs-lookup"><span data-stu-id="13025-133">assignments</span></span>|<span data-ttu-id="13025-134">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="13025-134">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="13025-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="13025-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="13025-136">応答</span><span class="sxs-lookup"><span data-stu-id="13025-136">Response</span></span>
<span data-ttu-id="13025-137">かどうか、成功を返すアクション、`200 OK`応答コードおよび応答の本文に[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="13025-137">If successful, this action returns a `200 OK` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13025-138">例</span><span class="sxs-lookup"><span data-stu-id="13025-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="13025-139">要求</span><span class="sxs-lookup"><span data-stu-id="13025-139">Request</span></span>
<span data-ttu-id="13025-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="13025-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assign

Content-type: application/json
Content-length: 287

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
      "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="13025-141">応答</span><span class="sxs-lookup"><span data-stu-id="13025-141">Response</span></span>
<span data-ttu-id="13025-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="13025-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 281

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
      "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





