---
title: syncMicrosoftStoreForBusinessApps アクション
description: ビジネス向け Microsoft Store と Intune アカウントを同期します
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e71bfb1e4ac6d4ce6c31344289eab7fb15b65594
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254269"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="8f409-103">syncMicrosoftStoreForBusinessApps アクション</span><span class="sxs-lookup"><span data-stu-id="8f409-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="8f409-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8f409-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f409-105">ビジネス向け Microsoft Store と Intune アカウントを同期する</span><span class="sxs-lookup"><span data-stu-id="8f409-105">Syncs Intune account with Microsoft Store For Business</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f409-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="8f409-106">Prerequisites</span></span>
<span data-ttu-id="8f409-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8f409-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f409-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8f409-109">Permission type</span></span>|<span data-ttu-id="8f409-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8f409-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f409-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8f409-111">Delegated (work or school account)</span></span>| 
| <span data-ttu-id="8f409-112">&nbsp; &nbsp; _オンボーディング_</span><span class="sxs-lookup"><span data-stu-id="8f409-112">&nbsp; &nbsp; _Onboarding_</span></span> | <span data-ttu-id="8f409-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f409-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8f409-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8f409-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f409-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8f409-115">Not supported.</span></span>|
|<span data-ttu-id="8f409-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8f409-116">Application</span></span>|<span data-ttu-id="8f409-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8f409-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f409-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8f409-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="8f409-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8f409-119">Request headers</span></span>
|<span data-ttu-id="8f409-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8f409-120">Header</span></span>|<span data-ttu-id="8f409-121">値</span><span class="sxs-lookup"><span data-stu-id="8f409-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f409-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f409-122">Authorization</span></span>|<span data-ttu-id="8f409-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8f409-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f409-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8f409-124">Accept</span></span>|<span data-ttu-id="8f409-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8f409-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f409-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8f409-126">Request body</span></span>
<span data-ttu-id="8f409-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8f409-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f409-128">応答</span><span class="sxs-lookup"><span data-stu-id="8f409-128">Response</span></span>
<span data-ttu-id="8f409-129">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="8f409-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example-request"></a><span data-ttu-id="8f409-130">要求の例</span><span class="sxs-lookup"><span data-stu-id="8f409-130">Example request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="8f409-131">応答</span><span class="sxs-lookup"><span data-stu-id="8f409-131">Response</span></span>

<span data-ttu-id="8f409-132">簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="8f409-132">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8f409-133">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8f409-133">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



