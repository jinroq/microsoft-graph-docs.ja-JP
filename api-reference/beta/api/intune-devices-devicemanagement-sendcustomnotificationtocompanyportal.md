---
title: sendCustomNotificationToCompanyPortal アクション
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 92276ac8609f1699b1b4a4217452f121d8507f47
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978852"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="37640-103">sendCustomNotificationToCompanyPortal アクション</span><span class="sxs-lookup"><span data-stu-id="37640-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="37640-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="37640-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="37640-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37640-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37640-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="37640-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="37640-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="37640-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="37640-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="37640-108">Prerequisites</span></span>
<span data-ttu-id="37640-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="37640-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37640-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="37640-111">Permission type</span></span>|<span data-ttu-id="37640-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="37640-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37640-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="37640-113">Delegated (work or school account)</span></span>|<span data-ttu-id="37640-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37640-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="37640-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="37640-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37640-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37640-116">Not supported.</span></span>|
|<span data-ttu-id="37640-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="37640-117">Application</span></span>|<span data-ttu-id="37640-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37640-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37640-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="37640-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="37640-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="37640-120">Request headers</span></span>
|<span data-ttu-id="37640-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="37640-121">Header</span></span>|<span data-ttu-id="37640-122">値</span><span class="sxs-lookup"><span data-stu-id="37640-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37640-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="37640-123">Authorization</span></span>|<span data-ttu-id="37640-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="37640-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37640-125">Accept</span><span class="sxs-lookup"><span data-stu-id="37640-125">Accept</span></span>|<span data-ttu-id="37640-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37640-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37640-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="37640-127">Request body</span></span>
<span data-ttu-id="37640-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="37640-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="37640-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="37640-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="37640-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="37640-130">Property</span></span>|<span data-ttu-id="37640-131">型</span><span class="sxs-lookup"><span data-stu-id="37640-131">Type</span></span>|<span data-ttu-id="37640-132">説明</span><span class="sxs-lookup"><span data-stu-id="37640-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37640-133">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="37640-133">notificationTitle</span></span>|<span data-ttu-id="37640-134">String</span><span class="sxs-lookup"><span data-stu-id="37640-134">String</span></span>|<span data-ttu-id="37640-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="37640-135">Not yet documented</span></span>|
|<span data-ttu-id="37640-136">notificationBody</span><span class="sxs-lookup"><span data-stu-id="37640-136">notificationBody</span></span>|<span data-ttu-id="37640-137">String</span><span class="sxs-lookup"><span data-stu-id="37640-137">String</span></span>|<span data-ttu-id="37640-138">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="37640-138">Not yet documented</span></span>|
|<span data-ttu-id="37640-139">groupsToNotify</span><span class="sxs-lookup"><span data-stu-id="37640-139">groupsToNotify</span></span>|<span data-ttu-id="37640-140">String コレクション</span><span class="sxs-lookup"><span data-stu-id="37640-140">String collection</span></span>|<span data-ttu-id="37640-141">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="37640-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="37640-142">応答</span><span class="sxs-lookup"><span data-stu-id="37640-142">Response</span></span>
<span data-ttu-id="37640-143">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="37640-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="37640-144">例</span><span class="sxs-lookup"><span data-stu-id="37640-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="37640-145">要求</span><span class="sxs-lookup"><span data-stu-id="37640-145">Request</span></span>
<span data-ttu-id="37640-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="37640-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="37640-147">応答</span><span class="sxs-lookup"><span data-stu-id="37640-147">Response</span></span>
<span data-ttu-id="37640-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="37640-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





