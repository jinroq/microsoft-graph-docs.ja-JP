---
title: updatePriorities アクション
description: ポリシーの優先度を更新します。
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: 1a237ac20154e9356ff999bc5c671b02c15c7028
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934055"
---
# <a name="updatepriorities-action"></a><span data-ttu-id="4cb16-103">updatePriorities アクション</span><span class="sxs-lookup"><span data-stu-id="4cb16-103">updatePriorities action</span></span>

> <span data-ttu-id="4cb16-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4cb16-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4cb16-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4cb16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cb16-106">ポリシーの優先度を更新します。</span><span class="sxs-lookup"><span data-stu-id="4cb16-106">Update policy priorities.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4cb16-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="4cb16-107">Prerequisites</span></span>
<span data-ttu-id="4cb16-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4cb16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cb16-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4cb16-110">Permission type</span></span>|<span data-ttu-id="4cb16-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4cb16-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4cb16-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4cb16-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4cb16-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cb16-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4cb16-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4cb16-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4cb16-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4cb16-115">Not supported.</span></span>|
|<span data-ttu-id="4cb16-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4cb16-116">Application</span></span>|<span data-ttu-id="4cb16-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4cb16-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4cb16-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4cb16-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities
```

## <a name="request-headers"></a><span data-ttu-id="4cb16-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4cb16-119">Request headers</span></span>
|<span data-ttu-id="4cb16-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4cb16-120">Header</span></span>|<span data-ttu-id="4cb16-121">値</span><span class="sxs-lookup"><span data-stu-id="4cb16-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4cb16-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4cb16-122">Authorization</span></span>|<span data-ttu-id="4cb16-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4cb16-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4cb16-124">承諾</span><span class="sxs-lookup"><span data-stu-id="4cb16-124">Accept</span></span>|<span data-ttu-id="4cb16-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4cb16-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cb16-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4cb16-126">Request body</span></span>
<span data-ttu-id="4cb16-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4cb16-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4cb16-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="4cb16-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4cb16-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4cb16-129">Property</span></span>|<span data-ttu-id="4cb16-130">型</span><span class="sxs-lookup"><span data-stu-id="4cb16-130">Type</span></span>|<span data-ttu-id="4cb16-131">説明</span><span class="sxs-lookup"><span data-stu-id="4cb16-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cb16-132">officeConfigurationPolicyIds</span><span class="sxs-lookup"><span data-stu-id="4cb16-132">officeConfigurationPolicyIds</span></span>|<span data-ttu-id="4cb16-133">String collection</span><span class="sxs-lookup"><span data-stu-id="4cb16-133">String collection</span></span>|<span data-ttu-id="4cb16-134">Office 構成ポリシー id の一覧</span><span class="sxs-lookup"><span data-stu-id="4cb16-134">List of office configuration policy ids</span></span>|
|<span data-ttu-id="4cb16-135">officeConfigurationPriorities</span><span class="sxs-lookup"><span data-stu-id="4cb16-135">officeConfigurationPriorities</span></span>|<span data-ttu-id="4cb16-136">Int32 コレクション</span><span class="sxs-lookup"><span data-stu-id="4cb16-136">Int32 collection</span></span>|<span data-ttu-id="4cb16-137">Office の構成の優先度の一覧</span><span class="sxs-lookup"><span data-stu-id="4cb16-137">List of office configuration priorities</span></span>|



## <a name="response"></a><span data-ttu-id="4cb16-138">応答</span><span class="sxs-lookup"><span data-stu-id="4cb16-138">Response</span></span>
<span data-ttu-id="4cb16-139">成功した場合、このアクションは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="4cb16-139">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4cb16-140">例</span><span class="sxs-lookup"><span data-stu-id="4cb16-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="4cb16-141">要求</span><span class="sxs-lookup"><span data-stu-id="4cb16-141">Request</span></span>
<span data-ttu-id="4cb16-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4cb16-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4cb16-143">応答</span><span class="sxs-lookup"><span data-stu-id="4cb16-143">Response</span></span>
<span data-ttu-id="4cb16-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4cb16-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```



