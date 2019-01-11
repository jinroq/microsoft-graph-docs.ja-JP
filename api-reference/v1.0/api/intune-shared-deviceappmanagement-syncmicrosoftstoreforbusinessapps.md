---
title: syncMicrosoftStoreForBusinessApps アクション
description: ビジネス向け Microsoft Store と Intune アカウントを同期します
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bba25378dae6f74104cb3ecc3a336404181b9a79
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821645"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="8a88c-103">syncMicrosoftStoreForBusinessApps アクション</span><span class="sxs-lookup"><span data-stu-id="8a88c-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="8a88c-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a88c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a88c-105">ビジネス向け Microsoft Store と Intune アカウントを同期する</span><span class="sxs-lookup"><span data-stu-id="8a88c-105">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8a88c-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="8a88c-106">Prerequisites</span></span>
<span data-ttu-id="8a88c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a88c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a88c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8a88c-109">Permission type</span></span>|<span data-ttu-id="8a88c-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8a88c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a88c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8a88c-111">Delegated (work or school account)</span></span>| 
| <span data-ttu-id="8a88c-112">&nbsp;&nbsp; _契約時_</span><span class="sxs-lookup"><span data-stu-id="8a88c-112">&nbsp; &nbsp; _Onboarding_</span></span> | <span data-ttu-id="8a88c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a88c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8a88c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8a88c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a88c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a88c-115">Not supported.</span></span>|
|<span data-ttu-id="8a88c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8a88c-116">Application</span></span>|<span data-ttu-id="8a88c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a88c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a88c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8a88c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="8a88c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a88c-119">Request headers</span></span>
|<span data-ttu-id="8a88c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a88c-120">Header</span></span>|<span data-ttu-id="8a88c-121">値</span><span class="sxs-lookup"><span data-stu-id="8a88c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a88c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a88c-122">Authorization</span></span>|<span data-ttu-id="8a88c-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8a88c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a88c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8a88c-124">Accept</span></span>|<span data-ttu-id="8a88c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8a88c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a88c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8a88c-126">Request body</span></span>
<span data-ttu-id="8a88c-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8a88c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a88c-128">応答</span><span class="sxs-lookup"><span data-stu-id="8a88c-128">Response</span></span>
<span data-ttu-id="8a88c-129">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="8a88c-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example-request"></a><span data-ttu-id="8a88c-130">要求の例</span><span class="sxs-lookup"><span data-stu-id="8a88c-130">Example request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="8a88c-131">応答</span><span class="sxs-lookup"><span data-stu-id="8a88c-131">Response</span></span>

<span data-ttu-id="8a88c-132">ここに示す応答オブジェクトは、簡潔にするために切り詰められます。</span><span class="sxs-lookup"><span data-stu-id="8a88c-132">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8a88c-133">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8a88c-133">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



