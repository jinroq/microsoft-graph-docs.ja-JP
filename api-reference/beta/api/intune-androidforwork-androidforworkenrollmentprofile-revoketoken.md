---
title: revokeToken アクション
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 111ba55f1268c5b630d6f2ea284d7f14db80cce8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36322822"
---
# <a name="revoketoken-action"></a><span data-ttu-id="e35f5-103">revokeToken アクション</span><span class="sxs-lookup"><span data-stu-id="e35f5-103">revokeToken action</span></span>

> <span data-ttu-id="e35f5-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e35f5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e35f5-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e35f5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e35f5-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e35f5-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e35f5-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e35f5-107">Prerequisites</span></span>
<span data-ttu-id="e35f5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e35f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e35f5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e35f5-110">Permission type</span></span>|<span data-ttu-id="e35f5-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e35f5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e35f5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e35f5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e35f5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e35f5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e35f5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e35f5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e35f5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e35f5-115">Not supported.</span></span>|
|<span data-ttu-id="e35f5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e35f5-116">Application</span></span>|<span data-ttu-id="e35f5-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e35f5-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e35f5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e35f5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}/revokeToken
```

## <a name="request-headers"></a><span data-ttu-id="e35f5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e35f5-119">Request headers</span></span>
|<span data-ttu-id="e35f5-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e35f5-120">Header</span></span>|<span data-ttu-id="e35f5-121">値</span><span class="sxs-lookup"><span data-stu-id="e35f5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e35f5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e35f5-122">Authorization</span></span>|<span data-ttu-id="e35f5-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e35f5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e35f5-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e35f5-124">Accept</span></span>|<span data-ttu-id="e35f5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e35f5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e35f5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e35f5-126">Request body</span></span>
<span data-ttu-id="e35f5-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e35f5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e35f5-128">応答</span><span class="sxs-lookup"><span data-stu-id="e35f5-128">Response</span></span>
<span data-ttu-id="e35f5-129">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="e35f5-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e35f5-130">例</span><span class="sxs-lookup"><span data-stu-id="e35f5-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e35f5-131">要求</span><span class="sxs-lookup"><span data-stu-id="e35f5-131">Request</span></span>
<span data-ttu-id="e35f5-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e35f5-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}/revokeToken
```

### <a name="response"></a><span data-ttu-id="e35f5-133">応答</span><span class="sxs-lookup"><span data-stu-id="e35f5-133">Response</span></span>
<span data-ttu-id="e35f5-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e35f5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






