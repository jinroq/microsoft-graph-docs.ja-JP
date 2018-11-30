---
title: sendCustomNotificationToCompanyPortal アクション
description: まだ文書化されていません
ms.openlocfilehash: bf19f87c385568a38407fff0df144c6df165fbc0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069052"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="4fb7e-103">sendCustomNotificationToCompanyPortal アクション</span><span class="sxs-lookup"><span data-stu-id="4fb7e-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="4fb7e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4fb7e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4fb7e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4fb7e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4fb7e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4fb7e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4fb7e-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4fb7e-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4fb7e-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="4fb7e-108">Prerequisites</span></span>
<span data-ttu-id="4fb7e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4fb7e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fb7e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4fb7e-111">Permission type</span></span>|<span data-ttu-id="4fb7e-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4fb7e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fb7e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4fb7e-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4fb7e-114">&nbsp; &nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="4fb7e-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="4fb7e-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fb7e-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4fb7e-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4fb7e-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fb7e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4fb7e-117">Not supported.</span></span>|
|<span data-ttu-id="4fb7e-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4fb7e-118">Application</span></span>|<span data-ttu-id="4fb7e-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4fb7e-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fb7e-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4fb7e-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="4fb7e-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4fb7e-121">Request headers</span></span>
|<span data-ttu-id="4fb7e-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4fb7e-122">Header</span></span>|<span data-ttu-id="4fb7e-123">値</span><span class="sxs-lookup"><span data-stu-id="4fb7e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fb7e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fb7e-124">Authorization</span></span>|<span data-ttu-id="4fb7e-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4fb7e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fb7e-126">Accept</span><span class="sxs-lookup"><span data-stu-id="4fb7e-126">Accept</span></span>|<span data-ttu-id="4fb7e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4fb7e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fb7e-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="4fb7e-128">Request body</span></span>
<span data-ttu-id="4fb7e-129">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4fb7e-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4fb7e-130">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="4fb7e-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4fb7e-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fb7e-131">Property</span></span>|<span data-ttu-id="4fb7e-132">型</span><span class="sxs-lookup"><span data-stu-id="4fb7e-132">Type</span></span>|<span data-ttu-id="4fb7e-133">説明</span><span class="sxs-lookup"><span data-stu-id="4fb7e-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fb7e-134">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="4fb7e-134">notificationTitle</span></span>|<span data-ttu-id="4fb7e-135">String</span><span class="sxs-lookup"><span data-stu-id="4fb7e-135">String</span></span>|<span data-ttu-id="4fb7e-136">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4fb7e-136">Not yet documented</span></span>|
|<span data-ttu-id="4fb7e-137">notificationBody</span><span class="sxs-lookup"><span data-stu-id="4fb7e-137">notificationBody</span></span>|<span data-ttu-id="4fb7e-138">String</span><span class="sxs-lookup"><span data-stu-id="4fb7e-138">String</span></span>|<span data-ttu-id="4fb7e-139">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4fb7e-139">Not yet documented</span></span>|
|<span data-ttu-id="4fb7e-140">groupsToNotify</span><span class="sxs-lookup"><span data-stu-id="4fb7e-140">groupsToNotify</span></span>|<span data-ttu-id="4fb7e-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="4fb7e-141">String collection</span></span>|<span data-ttu-id="4fb7e-142">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4fb7e-142">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4fb7e-143">応答</span><span class="sxs-lookup"><span data-stu-id="4fb7e-143">Response</span></span>
<span data-ttu-id="4fb7e-144">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="4fb7e-144">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4fb7e-145">例</span><span class="sxs-lookup"><span data-stu-id="4fb7e-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="4fb7e-146">要求</span><span class="sxs-lookup"><span data-stu-id="4fb7e-146">Request</span></span>
<span data-ttu-id="4fb7e-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4fb7e-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/sendCustomNotificationToCompanyPortal

Content-type: application/json
Content-length: 164

{
  "notificationTitle": "Notification Title value",
  "notificationBody": "Notification Body value",
  "groupsToNotify": [
    "Groups To Notify value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="4fb7e-148">応答</span><span class="sxs-lookup"><span data-stu-id="4fb7e-148">Response</span></span>
<span data-ttu-id="4fb7e-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4fb7e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






