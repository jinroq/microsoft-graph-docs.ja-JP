---
title: syncMicrosoftStoreForBusinessApps アクション
description: ビジネス向け Microsoft Store と Intune アカウントを同期します
author: tfitzmac
ms.openlocfilehash: 77171a96dd8a6b053234e9f95a8b79f4368abe4e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317984"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="0698e-103">syncMicrosoftStoreForBusinessApps アクション</span><span class="sxs-lookup"><span data-stu-id="0698e-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="0698e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0698e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0698e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0698e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0698e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0698e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0698e-107">ビジネス向け Microsoft Store と Intune アカウントを同期する</span><span class="sxs-lookup"><span data-stu-id="0698e-107">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0698e-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="0698e-108">Prerequisites</span></span>
<span data-ttu-id="0698e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0698e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0698e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0698e-111">Permission type</span></span>|<span data-ttu-id="0698e-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0698e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0698e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0698e-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0698e-114">&nbsp;&nbsp; **契約時**</span><span class="sxs-lookup"><span data-stu-id="0698e-114">&nbsp; &nbsp; **Onboarding**</span></span> | |<span data-ttu-id="0698e-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0698e-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0698e-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0698e-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0698e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0698e-117">Not supported.</span></span>|
|<span data-ttu-id="0698e-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0698e-118">Application</span></span>|<span data-ttu-id="0698e-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0698e-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0698e-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0698e-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="0698e-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0698e-121">Request headers</span></span>
|<span data-ttu-id="0698e-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0698e-122">Header</span></span>|<span data-ttu-id="0698e-123">値</span><span class="sxs-lookup"><span data-stu-id="0698e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0698e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0698e-124">Authorization</span></span>|<span data-ttu-id="0698e-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0698e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0698e-126">Accept</span><span class="sxs-lookup"><span data-stu-id="0698e-126">Accept</span></span>|<span data-ttu-id="0698e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0698e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0698e-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="0698e-128">Request body</span></span>
<span data-ttu-id="0698e-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0698e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0698e-130">応答</span><span class="sxs-lookup"><span data-stu-id="0698e-130">Response</span></span>
<span data-ttu-id="0698e-131">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="0698e-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0698e-132">例</span><span class="sxs-lookup"><span data-stu-id="0698e-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="0698e-133">要求</span><span class="sxs-lookup"><span data-stu-id="0698e-133">Request</span></span>
<span data-ttu-id="0698e-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0698e-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="0698e-135">応答</span><span class="sxs-lookup"><span data-stu-id="0698e-135">Response</span></span>
<span data-ttu-id="0698e-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0698e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



