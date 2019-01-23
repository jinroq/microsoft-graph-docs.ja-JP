---
title: updatePriorities アクション
description: ポリシーの優先順位を更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a78ec2801522354709643dfdd88da0e6dd9756c8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412976"
---
# <a name="updatepriorities-action"></a><span data-ttu-id="4508b-103">updatePriorities アクション</span><span class="sxs-lookup"><span data-stu-id="4508b-103">updatePriorities action</span></span>

> <span data-ttu-id="4508b-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4508b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4508b-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4508b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4508b-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4508b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4508b-107">ポリシーの優先順位を更新します。</span><span class="sxs-lookup"><span data-stu-id="4508b-107">Update policy priorities.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4508b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="4508b-108">Prerequisites</span></span>
<span data-ttu-id="4508b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4508b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4508b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4508b-111">Permission type</span></span>|<span data-ttu-id="4508b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4508b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4508b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4508b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4508b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4508b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4508b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4508b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4508b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4508b-116">Not supported.</span></span>|
|<span data-ttu-id="4508b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4508b-117">Application</span></span>|<span data-ttu-id="4508b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4508b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4508b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4508b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities
```

## <a name="request-headers"></a><span data-ttu-id="4508b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4508b-120">Request headers</span></span>
|<span data-ttu-id="4508b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4508b-121">Header</span></span>|<span data-ttu-id="4508b-122">値</span><span class="sxs-lookup"><span data-stu-id="4508b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4508b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4508b-123">Authorization</span></span>|<span data-ttu-id="4508b-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4508b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4508b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4508b-125">Accept</span></span>|<span data-ttu-id="4508b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4508b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4508b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4508b-127">Request body</span></span>
<span data-ttu-id="4508b-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4508b-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4508b-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="4508b-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4508b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4508b-130">Property</span></span>|<span data-ttu-id="4508b-131">型</span><span class="sxs-lookup"><span data-stu-id="4508b-131">Type</span></span>|<span data-ttu-id="4508b-132">説明</span><span class="sxs-lookup"><span data-stu-id="4508b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4508b-133">officeConfigurationPolicyIds</span><span class="sxs-lookup"><span data-stu-id="4508b-133">officeConfigurationPolicyIds</span></span>|<span data-ttu-id="4508b-134">String コレクション</span><span class="sxs-lookup"><span data-stu-id="4508b-134">String collection</span></span>|<span data-ttu-id="4508b-135">Office の構成のポリシー id のリスト</span><span class="sxs-lookup"><span data-stu-id="4508b-135">List of office configuration policy ids</span></span>|
|<span data-ttu-id="4508b-136">officeConfigurationPriorities</span><span class="sxs-lookup"><span data-stu-id="4508b-136">officeConfigurationPriorities</span></span>|<span data-ttu-id="4508b-137">Int32 型のコレクション</span><span class="sxs-lookup"><span data-stu-id="4508b-137">Int32 collection</span></span>|<span data-ttu-id="4508b-138">Office 設定の優先順位の一覧</span><span class="sxs-lookup"><span data-stu-id="4508b-138">List of office configuration priorities</span></span>|



## <a name="response"></a><span data-ttu-id="4508b-139">応答</span><span class="sxs-lookup"><span data-stu-id="4508b-139">Response</span></span>
<span data-ttu-id="4508b-140">成功した場合、このアクションは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="4508b-140">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4508b-141">例</span><span class="sxs-lookup"><span data-stu-id="4508b-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="4508b-142">要求</span><span class="sxs-lookup"><span data-stu-id="4508b-142">Request</span></span>
<span data-ttu-id="4508b-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4508b-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4508b-144">応答</span><span class="sxs-lookup"><span data-stu-id="4508b-144">Response</span></span>
<span data-ttu-id="4508b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4508b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```



