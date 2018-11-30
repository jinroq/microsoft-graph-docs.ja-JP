---
title: revokeLicenses アクション
description: 特定の appleVolumePurchaseProgramToken に関連付けられているライセンスを失効させる
ms.openlocfilehash: 9c8d3142a28845390ef7261c408d2d4bc77643c1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068342"
---
# <a name="revokelicenses-action"></a><span data-ttu-id="3e811-103">revokeLicenses アクション</span><span class="sxs-lookup"><span data-stu-id="3e811-103">revokeLicenses action</span></span>

> <span data-ttu-id="3e811-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3e811-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e811-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3e811-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3e811-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3e811-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3e811-107">特定の appleVolumePurchaseProgramToken に関連付けられているライセンスを失効させる</span><span class="sxs-lookup"><span data-stu-id="3e811-107">Revoke licenses associated with a specific appleVolumePurchaseProgramToken</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3e811-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="3e811-108">Prerequisites</span></span>
<span data-ttu-id="3e811-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3e811-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e811-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3e811-111">Permission type</span></span>|<span data-ttu-id="3e811-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3e811-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e811-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3e811-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3e811-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e811-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3e811-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3e811-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e811-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3e811-116">Not supported.</span></span>|
|<span data-ttu-id="3e811-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3e811-117">Application</span></span>|<span data-ttu-id="3e811-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3e811-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e811-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3e811-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/revokeLicenses
```

## <a name="request-headers"></a><span data-ttu-id="3e811-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3e811-120">Request headers</span></span>
|<span data-ttu-id="3e811-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3e811-121">Header</span></span>|<span data-ttu-id="3e811-122">値</span><span class="sxs-lookup"><span data-stu-id="3e811-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e811-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e811-123">Authorization</span></span>|<span data-ttu-id="3e811-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3e811-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e811-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3e811-125">Accept</span></span>|<span data-ttu-id="3e811-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3e811-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e811-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3e811-127">Request body</span></span>
<span data-ttu-id="3e811-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3e811-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3e811-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="3e811-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3e811-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3e811-130">Property</span></span>|<span data-ttu-id="3e811-131">型</span><span class="sxs-lookup"><span data-stu-id="3e811-131">Type</span></span>|<span data-ttu-id="3e811-132">説明</span><span class="sxs-lookup"><span data-stu-id="3e811-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e811-133">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="3e811-133">notifyManagedDevices</span></span>|<span data-ttu-id="3e811-134">ブール値</span><span class="sxs-lookup"><span data-stu-id="3e811-134">Boolean</span></span>|<span data-ttu-id="3e811-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3e811-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3e811-136">応答</span><span class="sxs-lookup"><span data-stu-id="3e811-136">Response</span></span>
<span data-ttu-id="3e811-137">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="3e811-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3e811-138">例</span><span class="sxs-lookup"><span data-stu-id="3e811-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="3e811-139">要求</span><span class="sxs-lookup"><span data-stu-id="3e811-139">Request</span></span>
<span data-ttu-id="3e811-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3e811-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/revokeLicenses

Content-type: application/json
Content-length: 36

{
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="3e811-141">応答</span><span class="sxs-lookup"><span data-stu-id="3e811-141">Response</span></span>
<span data-ttu-id="3e811-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3e811-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




