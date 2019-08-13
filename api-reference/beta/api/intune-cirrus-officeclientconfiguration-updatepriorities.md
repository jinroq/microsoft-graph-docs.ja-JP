---
title: updatePriorities アクション
description: ポリシーの優先度を更新します。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a236a20c6563f8ddb0b464168d7fb7d5e5d7ac43
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328282"
---
# <a name="updatepriorities-action"></a><span data-ttu-id="19c5a-103">updatePriorities アクション</span><span class="sxs-lookup"><span data-stu-id="19c5a-103">updatePriorities action</span></span>

> <span data-ttu-id="19c5a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19c5a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19c5a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="19c5a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19c5a-106">ポリシーの優先度を更新します。</span><span class="sxs-lookup"><span data-stu-id="19c5a-106">Update policy priorities.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19c5a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="19c5a-107">Prerequisites</span></span>
<span data-ttu-id="19c5a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="19c5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19c5a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="19c5a-110">Permission type</span></span>|<span data-ttu-id="19c5a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="19c5a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19c5a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="19c5a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="19c5a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19c5a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="19c5a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="19c5a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19c5a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19c5a-115">Not supported.</span></span>|
|<span data-ttu-id="19c5a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="19c5a-116">Application</span></span>|<span data-ttu-id="19c5a-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19c5a-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="19c5a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="19c5a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities
```

## <a name="request-headers"></a><span data-ttu-id="19c5a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="19c5a-119">Request headers</span></span>
|<span data-ttu-id="19c5a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="19c5a-120">Header</span></span>|<span data-ttu-id="19c5a-121">値</span><span class="sxs-lookup"><span data-stu-id="19c5a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19c5a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="19c5a-122">Authorization</span></span>|<span data-ttu-id="19c5a-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="19c5a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19c5a-124">承諾</span><span class="sxs-lookup"><span data-stu-id="19c5a-124">Accept</span></span>|<span data-ttu-id="19c5a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="19c5a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19c5a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="19c5a-126">Request body</span></span>
<span data-ttu-id="19c5a-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="19c5a-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="19c5a-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="19c5a-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="19c5a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="19c5a-129">Property</span></span>|<span data-ttu-id="19c5a-130">型</span><span class="sxs-lookup"><span data-stu-id="19c5a-130">Type</span></span>|<span data-ttu-id="19c5a-131">説明</span><span class="sxs-lookup"><span data-stu-id="19c5a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19c5a-132">officeConfigurationPolicyIds</span><span class="sxs-lookup"><span data-stu-id="19c5a-132">officeConfigurationPolicyIds</span></span>|<span data-ttu-id="19c5a-133">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="19c5a-133">String collection</span></span>|<span data-ttu-id="19c5a-134">Office 構成ポリシー id の一覧</span><span class="sxs-lookup"><span data-stu-id="19c5a-134">List of office configuration policy ids</span></span>|
|<span data-ttu-id="19c5a-135">officeConfigurationPriorities</span><span class="sxs-lookup"><span data-stu-id="19c5a-135">officeConfigurationPriorities</span></span>|<span data-ttu-id="19c5a-136">Int32 コレクション</span><span class="sxs-lookup"><span data-stu-id="19c5a-136">Int32 collection</span></span>|<span data-ttu-id="19c5a-137">Office の構成の優先度の一覧</span><span class="sxs-lookup"><span data-stu-id="19c5a-137">List of office configuration priorities</span></span>|



## <a name="response"></a><span data-ttu-id="19c5a-138">応答</span><span class="sxs-lookup"><span data-stu-id="19c5a-138">Response</span></span>
<span data-ttu-id="19c5a-139">成功した場合、このアクションは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="19c5a-139">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="19c5a-140">例</span><span class="sxs-lookup"><span data-stu-id="19c5a-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="19c5a-141">要求</span><span class="sxs-lookup"><span data-stu-id="19c5a-141">Request</span></span>
<span data-ttu-id="19c5a-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="19c5a-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities

Content-type: application/json
Content-length: 143

{
  "officeConfigurationPolicyIds": [
    "Office Configuration Policy Ids value"
  ],
  "officeConfigurationPriorities": [
    13
  ]
}
```

### <a name="response"></a><span data-ttu-id="19c5a-143">応答</span><span class="sxs-lookup"><span data-stu-id="19c5a-143">Response</span></span>
<span data-ttu-id="19c5a-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="19c5a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```






