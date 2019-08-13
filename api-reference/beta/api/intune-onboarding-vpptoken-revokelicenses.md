---
title: revokeLicenses アクション
description: 特定の appleVolumePurchaseProgramToken に関連付けられているライセンスを取り消す
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 73d4f82899d3b7cda27e02418f2d140cea828834
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36352274"
---
# <a name="revokelicenses-action"></a><span data-ttu-id="65ff9-103">revokeLicenses アクション</span><span class="sxs-lookup"><span data-stu-id="65ff9-103">revokeLicenses action</span></span>

> <span data-ttu-id="65ff9-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65ff9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65ff9-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="65ff9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65ff9-106">特定の appleVolumePurchaseProgramToken に関連付けられているライセンスを取り消す</span><span class="sxs-lookup"><span data-stu-id="65ff9-106">Revoke licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65ff9-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="65ff9-107">Prerequisites</span></span>
<span data-ttu-id="65ff9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65ff9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65ff9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="65ff9-110">Permission type</span></span>|<span data-ttu-id="65ff9-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="65ff9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65ff9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="65ff9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="65ff9-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65ff9-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="65ff9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="65ff9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65ff9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65ff9-115">Not supported.</span></span>|
|<span data-ttu-id="65ff9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="65ff9-116">Application</span></span>|<span data-ttu-id="65ff9-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65ff9-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="65ff9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="65ff9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/revokeLicenses
```

## <a name="request-headers"></a><span data-ttu-id="65ff9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="65ff9-119">Request headers</span></span>
|<span data-ttu-id="65ff9-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="65ff9-120">Header</span></span>|<span data-ttu-id="65ff9-121">値</span><span class="sxs-lookup"><span data-stu-id="65ff9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65ff9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="65ff9-122">Authorization</span></span>|<span data-ttu-id="65ff9-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="65ff9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65ff9-124">承諾</span><span class="sxs-lookup"><span data-stu-id="65ff9-124">Accept</span></span>|<span data-ttu-id="65ff9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="65ff9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65ff9-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="65ff9-126">Request body</span></span>
<span data-ttu-id="65ff9-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="65ff9-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="65ff9-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="65ff9-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="65ff9-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65ff9-129">Property</span></span>|<span data-ttu-id="65ff9-130">型</span><span class="sxs-lookup"><span data-stu-id="65ff9-130">Type</span></span>|<span data-ttu-id="65ff9-131">説明</span><span class="sxs-lookup"><span data-stu-id="65ff9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65ff9-132">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="65ff9-132">notifyManagedDevices</span></span>|<span data-ttu-id="65ff9-133">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="65ff9-133">Boolean</span></span>|<span data-ttu-id="65ff9-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="65ff9-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="65ff9-135">応答</span><span class="sxs-lookup"><span data-stu-id="65ff9-135">Response</span></span>
<span data-ttu-id="65ff9-136">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="65ff9-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="65ff9-137">例</span><span class="sxs-lookup"><span data-stu-id="65ff9-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="65ff9-138">要求</span><span class="sxs-lookup"><span data-stu-id="65ff9-138">Request</span></span>
<span data-ttu-id="65ff9-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="65ff9-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/revokeLicenses

Content-type: application/json
Content-length: 36

{
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="65ff9-140">応答</span><span class="sxs-lookup"><span data-stu-id="65ff9-140">Response</span></span>
<span data-ttu-id="65ff9-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="65ff9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






