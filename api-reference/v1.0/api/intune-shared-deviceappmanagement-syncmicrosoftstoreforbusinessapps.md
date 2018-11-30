---
title: syncMicrosoftStoreForBusinessApps アクション
description: ビジネス向け Microsoft Store と Intune アカウントを同期します
ms.openlocfilehash: a293c170dea23469b12a8862b8510fe8ce67be41
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022225"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="138bd-103">syncMicrosoftStoreForBusinessApps アクション</span><span class="sxs-lookup"><span data-stu-id="138bd-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="138bd-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="138bd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="138bd-105">ビジネス向け Microsoft Store と Intune アカウントを同期する</span><span class="sxs-lookup"><span data-stu-id="138bd-105">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="138bd-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="138bd-106">Prerequisites</span></span>
<span data-ttu-id="138bd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="138bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="138bd-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="138bd-109">Permission type</span></span>|<span data-ttu-id="138bd-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="138bd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="138bd-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="138bd-111">Delegated (work or school account)</span></span>| 
| <span data-ttu-id="138bd-112">&nbsp;&nbsp; _契約時_</span><span class="sxs-lookup"><span data-stu-id="138bd-112">&nbsp; &nbsp; _Onboarding_</span></span> | <span data-ttu-id="138bd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="138bd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="138bd-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="138bd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="138bd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="138bd-115">Not supported.</span></span>|
|<span data-ttu-id="138bd-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="138bd-116">Application</span></span>|<span data-ttu-id="138bd-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="138bd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="138bd-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="138bd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="138bd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="138bd-119">Request headers</span></span>
|<span data-ttu-id="138bd-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="138bd-120">Header</span></span>|<span data-ttu-id="138bd-121">値</span><span class="sxs-lookup"><span data-stu-id="138bd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="138bd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="138bd-122">Authorization</span></span>|<span data-ttu-id="138bd-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="138bd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="138bd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="138bd-124">Accept</span></span>|<span data-ttu-id="138bd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="138bd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="138bd-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="138bd-126">Request body</span></span>
<span data-ttu-id="138bd-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="138bd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="138bd-128">応答</span><span class="sxs-lookup"><span data-stu-id="138bd-128">Response</span></span>
<span data-ttu-id="138bd-129">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="138bd-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example-request"></a><span data-ttu-id="138bd-130">要求の例</span><span class="sxs-lookup"><span data-stu-id="138bd-130">Example request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="138bd-131">応答</span><span class="sxs-lookup"><span data-stu-id="138bd-131">Response</span></span>

<span data-ttu-id="138bd-132">ここに示す応答オブジェクトは、簡潔にするために切り詰められます。</span><span class="sxs-lookup"><span data-stu-id="138bd-132">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="138bd-133">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="138bd-133">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



