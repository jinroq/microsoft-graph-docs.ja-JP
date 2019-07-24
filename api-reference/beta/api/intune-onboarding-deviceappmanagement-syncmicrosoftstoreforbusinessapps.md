---
title: syncMicrosoftStoreForBusinessApps アクション
description: ビジネス向け Microsoft Store と Intune アカウントを同期する
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 12fb8ebe1f9405a7a318649129c7dc7875bd9dce
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741440"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="4070b-103">syncMicrosoftStoreForBusinessApps アクション</span><span class="sxs-lookup"><span data-stu-id="4070b-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="4070b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4070b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4070b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4070b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4070b-106">ビジネス向け Microsoft Store と Intune アカウントを同期する</span><span class="sxs-lookup"><span data-stu-id="4070b-106">Syncs Intune account with Microsoft Store For Business</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4070b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="4070b-107">Prerequisites</span></span>
<span data-ttu-id="4070b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4070b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4070b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4070b-110">Permission type</span></span>|<span data-ttu-id="4070b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4070b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4070b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4070b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4070b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4070b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4070b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4070b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4070b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4070b-115">Not supported.</span></span>|
|<span data-ttu-id="4070b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4070b-116">Application</span></span>|<span data-ttu-id="4070b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4070b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4070b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4070b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="4070b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4070b-119">Request headers</span></span>
|<span data-ttu-id="4070b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4070b-120">Header</span></span>|<span data-ttu-id="4070b-121">値</span><span class="sxs-lookup"><span data-stu-id="4070b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4070b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4070b-122">Authorization</span></span>|<span data-ttu-id="4070b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4070b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4070b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="4070b-124">Accept</span></span>|<span data-ttu-id="4070b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4070b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4070b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4070b-126">Request body</span></span>
<span data-ttu-id="4070b-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4070b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4070b-128">応答</span><span class="sxs-lookup"><span data-stu-id="4070b-128">Response</span></span>
<span data-ttu-id="4070b-129">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="4070b-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4070b-130">例</span><span class="sxs-lookup"><span data-stu-id="4070b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4070b-131">要求</span><span class="sxs-lookup"><span data-stu-id="4070b-131">Request</span></span>
<span data-ttu-id="4070b-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4070b-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="4070b-133">応答</span><span class="sxs-lookup"><span data-stu-id="4070b-133">Response</span></span>
<span data-ttu-id="4070b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4070b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




