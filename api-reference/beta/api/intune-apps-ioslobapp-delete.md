---
title: iosLobApp の削除
description: iosLobApp を削除します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5a64d4589ea53970e43d2176abddc4ee7e924bfa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864387"
---
# <a name="delete-ioslobapp"></a><span data-ttu-id="e1bc3-103">iosLobApp の削除</span><span class="sxs-lookup"><span data-stu-id="e1bc3-103">Delete iosLobApp</span></span>

> <span data-ttu-id="e1bc3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e1bc3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1bc3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1bc3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e1bc3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e1bc3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1bc3-107">[iosLobApp](../resources/intune-apps-ioslobapp.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="e1bc3-107">Deletes a [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e1bc3-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="e1bc3-108">Prerequisites</span></span>
<span data-ttu-id="e1bc3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e1bc3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1bc3-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e1bc3-111">Permission type</span></span>|<span data-ttu-id="e1bc3-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e1bc3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1bc3-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e1bc3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1bc3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1bc3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e1bc3-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e1bc3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1bc3-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1bc3-116">Not supported.</span></span>|
|<span data-ttu-id="e1bc3-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e1bc3-117">Application</span></span>|<span data-ttu-id="e1bc3-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1bc3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1bc3-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e1bc3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="e1bc3-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e1bc3-120">Request headers</span></span>
|<span data-ttu-id="e1bc3-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e1bc3-121">Header</span></span>|<span data-ttu-id="e1bc3-122">値</span><span class="sxs-lookup"><span data-stu-id="e1bc3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1bc3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1bc3-123">Authorization</span></span>|<span data-ttu-id="e1bc3-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e1bc3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1bc3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e1bc3-125">Accept</span></span>|<span data-ttu-id="e1bc3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1bc3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1bc3-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e1bc3-127">Request body</span></span>
<span data-ttu-id="e1bc3-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e1bc3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1bc3-129">応答</span><span class="sxs-lookup"><span data-stu-id="e1bc3-129">Response</span></span>
<span data-ttu-id="e1bc3-130">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="e1bc3-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e1bc3-131">例</span><span class="sxs-lookup"><span data-stu-id="e1bc3-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e1bc3-132">要求</span><span class="sxs-lookup"><span data-stu-id="e1bc3-132">Request</span></span>
<span data-ttu-id="e1bc3-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e1bc3-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="e1bc3-134">応答</span><span class="sxs-lookup"><span data-stu-id="e1bc3-134">Response</span></span>
<span data-ttu-id="e1bc3-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e1bc3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





