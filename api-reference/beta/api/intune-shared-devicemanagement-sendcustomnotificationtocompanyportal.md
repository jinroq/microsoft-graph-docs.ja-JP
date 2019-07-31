---
title: sendCustomNotificationToCompanyPortal アクション
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d6448cb70bcca6676b3662efb1cee6ad37351764
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979786"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="0ff36-103">sendCustomNotificationToCompanyPortal アクション</span><span class="sxs-lookup"><span data-stu-id="0ff36-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="0ff36-104">**重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0ff36-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0ff36-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ff36-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ff36-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0ff36-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ff36-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0ff36-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0ff36-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="0ff36-108">Prerequisites</span></span>
<span data-ttu-id="0ff36-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0ff36-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ff36-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0ff36-111">Permission type</span></span>|<span data-ttu-id="0ff36-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0ff36-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ff36-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0ff36-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0ff36-114">&nbsp;&nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="0ff36-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="0ff36-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ff36-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0ff36-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0ff36-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ff36-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ff36-117">Not supported.</span></span>|
|<span data-ttu-id="0ff36-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0ff36-118">Application</span></span>|<span data-ttu-id="0ff36-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ff36-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ff36-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0ff36-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="0ff36-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0ff36-121">Request headers</span></span>
|<span data-ttu-id="0ff36-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0ff36-122">Header</span></span>|<span data-ttu-id="0ff36-123">値</span><span class="sxs-lookup"><span data-stu-id="0ff36-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ff36-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ff36-124">Authorization</span></span>|<span data-ttu-id="0ff36-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0ff36-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ff36-126">承諾</span><span class="sxs-lookup"><span data-stu-id="0ff36-126">Accept</span></span>|<span data-ttu-id="0ff36-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0ff36-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ff36-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="0ff36-128">Request body</span></span>
<span data-ttu-id="0ff36-129">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0ff36-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0ff36-130">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="0ff36-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0ff36-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0ff36-131">Property</span></span>|<span data-ttu-id="0ff36-132">型</span><span class="sxs-lookup"><span data-stu-id="0ff36-132">Type</span></span>|<span data-ttu-id="0ff36-133">説明</span><span class="sxs-lookup"><span data-stu-id="0ff36-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ff36-134">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="0ff36-134">notificationTitle</span></span>|<span data-ttu-id="0ff36-135">String</span><span class="sxs-lookup"><span data-stu-id="0ff36-135">String</span></span>|<span data-ttu-id="0ff36-136">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0ff36-136">Not yet documented</span></span>|
|<span data-ttu-id="0ff36-137">notificationBody</span><span class="sxs-lookup"><span data-stu-id="0ff36-137">notificationBody</span></span>|<span data-ttu-id="0ff36-138">String</span><span class="sxs-lookup"><span data-stu-id="0ff36-138">String</span></span>|<span data-ttu-id="0ff36-139">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0ff36-139">Not yet documented</span></span>|
|<span data-ttu-id="0ff36-140">groupsToNotify</span><span class="sxs-lookup"><span data-stu-id="0ff36-140">groupsToNotify</span></span>|<span data-ttu-id="0ff36-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0ff36-141">String collection</span></span>|<span data-ttu-id="0ff36-142">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0ff36-142">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0ff36-143">応答</span><span class="sxs-lookup"><span data-stu-id="0ff36-143">Response</span></span>
<span data-ttu-id="0ff36-144">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="0ff36-144">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0ff36-145">例</span><span class="sxs-lookup"><span data-stu-id="0ff36-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="0ff36-146">要求</span><span class="sxs-lookup"><span data-stu-id="0ff36-146">Request</span></span>
<span data-ttu-id="0ff36-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0ff36-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0ff36-148">応答</span><span class="sxs-lookup"><span data-stu-id="0ff36-148">Response</span></span>
<span data-ttu-id="0ff36-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0ff36-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






