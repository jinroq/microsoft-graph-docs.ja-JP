---
title: syncMicrosoftStoreForBusinessApps アクション
description: ビジネス向け Microsoft Store と Intune アカウントを同期します
author: tfitzmac
ms.openlocfilehash: b26b379631cf5b28594e3cf247b735d6118e9b40
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354335"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="8a3c7-103">syncMicrosoftStoreForBusinessApps アクション</span><span class="sxs-lookup"><span data-stu-id="8a3c7-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="8a3c7-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a3c7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a3c7-105">ビジネス向け Microsoft Store と Intune アカウントを同期する</span><span class="sxs-lookup"><span data-stu-id="8a3c7-105">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8a3c7-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="8a3c7-106">Prerequisites</span></span>
<span data-ttu-id="8a3c7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a3c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a3c7-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8a3c7-109">Permission type</span></span>|<span data-ttu-id="8a3c7-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8a3c7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a3c7-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8a3c7-111">Delegated (work or school account)</span></span>| 
| <span data-ttu-id="8a3c7-112">&nbsp;&nbsp; _契約時_</span><span class="sxs-lookup"><span data-stu-id="8a3c7-112">&nbsp; &nbsp; _Onboarding_</span></span> | <span data-ttu-id="8a3c7-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a3c7-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8a3c7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8a3c7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a3c7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a3c7-115">Not supported.</span></span>|
|<span data-ttu-id="8a3c7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8a3c7-116">Application</span></span>|<span data-ttu-id="8a3c7-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a3c7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a3c7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8a3c7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="8a3c7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a3c7-119">Request headers</span></span>
|<span data-ttu-id="8a3c7-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a3c7-120">Header</span></span>|<span data-ttu-id="8a3c7-121">値</span><span class="sxs-lookup"><span data-stu-id="8a3c7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a3c7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a3c7-122">Authorization</span></span>|<span data-ttu-id="8a3c7-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8a3c7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a3c7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8a3c7-124">Accept</span></span>|<span data-ttu-id="8a3c7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8a3c7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a3c7-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8a3c7-126">Request body</span></span>
<span data-ttu-id="8a3c7-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8a3c7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a3c7-128">応答</span><span class="sxs-lookup"><span data-stu-id="8a3c7-128">Response</span></span>
<span data-ttu-id="8a3c7-129">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="8a3c7-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example-request"></a><span data-ttu-id="8a3c7-130">要求の例</span><span class="sxs-lookup"><span data-stu-id="8a3c7-130">Example request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="8a3c7-131">応答</span><span class="sxs-lookup"><span data-stu-id="8a3c7-131">Response</span></span>

<span data-ttu-id="8a3c7-132">ここに示す応答オブジェクトは、簡潔にするために切り詰められます。</span><span class="sxs-lookup"><span data-stu-id="8a3c7-132">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8a3c7-133">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8a3c7-133">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



