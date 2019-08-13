---
title: migrateToTemplate アクション
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 37e67efff5aef17b82a033e2b76dbeed707e072a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313273"
---
# <a name="migratetotemplate-action"></a><span data-ttu-id="48824-103">migrateToTemplate アクション</span><span class="sxs-lookup"><span data-stu-id="48824-103">migrateToTemplate action</span></span>

> <span data-ttu-id="48824-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48824-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48824-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="48824-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48824-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="48824-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48824-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="48824-107">Prerequisites</span></span>
<span data-ttu-id="48824-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="48824-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48824-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="48824-110">Permission type</span></span>|<span data-ttu-id="48824-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="48824-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48824-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="48824-112">Delegated (work or school account)</span></span>|<span data-ttu-id="48824-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48824-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="48824-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="48824-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48824-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48824-115">Not supported.</span></span>|
|<span data-ttu-id="48824-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="48824-116">Application</span></span>|<span data-ttu-id="48824-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48824-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="48824-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="48824-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/migrateToTemplate
```

## <a name="request-headers"></a><span data-ttu-id="48824-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="48824-119">Request headers</span></span>
|<span data-ttu-id="48824-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="48824-120">Header</span></span>|<span data-ttu-id="48824-121">値</span><span class="sxs-lookup"><span data-stu-id="48824-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48824-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="48824-122">Authorization</span></span>|<span data-ttu-id="48824-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="48824-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48824-124">承諾</span><span class="sxs-lookup"><span data-stu-id="48824-124">Accept</span></span>|<span data-ttu-id="48824-125">application/json</span><span class="sxs-lookup"><span data-stu-id="48824-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48824-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="48824-126">Request body</span></span>
<span data-ttu-id="48824-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="48824-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="48824-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="48824-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="48824-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48824-129">Property</span></span>|<span data-ttu-id="48824-130">型</span><span class="sxs-lookup"><span data-stu-id="48824-130">Type</span></span>|<span data-ttu-id="48824-131">説明</span><span class="sxs-lookup"><span data-stu-id="48824-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48824-132">newTemplateId</span><span class="sxs-lookup"><span data-stu-id="48824-132">newTemplateId</span></span>|<span data-ttu-id="48824-133">String</span><span class="sxs-lookup"><span data-stu-id="48824-133">String</span></span>|<span data-ttu-id="48824-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="48824-134">Not yet documented</span></span>|
|<span data-ttu-id="48824-135">preserveCustomValues</span><span class="sxs-lookup"><span data-stu-id="48824-135">preserveCustomValues</span></span>|<span data-ttu-id="48824-136">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="48824-136">Boolean</span></span>|<span data-ttu-id="48824-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="48824-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="48824-138">応答</span><span class="sxs-lookup"><span data-stu-id="48824-138">Response</span></span>
<span data-ttu-id="48824-139">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="48824-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="48824-140">例</span><span class="sxs-lookup"><span data-stu-id="48824-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="48824-141">要求</span><span class="sxs-lookup"><span data-stu-id="48824-141">Request</span></span>
<span data-ttu-id="48824-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="48824-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/migrateToTemplate

Content-type: application/json
Content-length: 81

{
  "newTemplateId": "New Template Id value",
  "preserveCustomValues": true
}
```

### <a name="response"></a><span data-ttu-id="48824-143">応答</span><span class="sxs-lookup"><span data-stu-id="48824-143">Response</span></span>
<span data-ttu-id="48824-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="48824-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






