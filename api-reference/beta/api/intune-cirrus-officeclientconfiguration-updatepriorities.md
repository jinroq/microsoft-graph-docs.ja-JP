---
title: updatePriorities アクション
description: ポリシーの優先順位を更新します。
ms.openlocfilehash: 23f41214b0dbbbdbf5949edea8857f8623ef0208
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073714"
---
# <a name="updatepriorities-action"></a><span data-ttu-id="0d95a-103">updatePriorities アクション</span><span class="sxs-lookup"><span data-stu-id="0d95a-103">updatePriorities action</span></span>

> <span data-ttu-id="0d95a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0d95a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d95a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d95a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0d95a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0d95a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0d95a-107">ポリシーの優先順位を更新します。</span><span class="sxs-lookup"><span data-stu-id="0d95a-107">Update policy priorities.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0d95a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="0d95a-108">Prerequisites</span></span>
<span data-ttu-id="0d95a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0d95a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d95a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0d95a-111">Permission type</span></span>|<span data-ttu-id="0d95a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0d95a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d95a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0d95a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0d95a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d95a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0d95a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0d95a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d95a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d95a-116">Not supported.</span></span>|
|<span data-ttu-id="0d95a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0d95a-117">Application</span></span>|<span data-ttu-id="0d95a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d95a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d95a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0d95a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities
```

## <a name="request-headers"></a><span data-ttu-id="0d95a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0d95a-120">Request headers</span></span>
|<span data-ttu-id="0d95a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0d95a-121">Header</span></span>|<span data-ttu-id="0d95a-122">値</span><span class="sxs-lookup"><span data-stu-id="0d95a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d95a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d95a-123">Authorization</span></span>|<span data-ttu-id="0d95a-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0d95a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d95a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0d95a-125">Accept</span></span>|<span data-ttu-id="0d95a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d95a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d95a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0d95a-127">Request body</span></span>
<span data-ttu-id="0d95a-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0d95a-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0d95a-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="0d95a-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0d95a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d95a-130">Property</span></span>|<span data-ttu-id="0d95a-131">型</span><span class="sxs-lookup"><span data-stu-id="0d95a-131">Type</span></span>|<span data-ttu-id="0d95a-132">説明</span><span class="sxs-lookup"><span data-stu-id="0d95a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d95a-133">officeConfigurationPolicyIds</span><span class="sxs-lookup"><span data-stu-id="0d95a-133">officeConfigurationPolicyIds</span></span>|<span data-ttu-id="0d95a-134">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0d95a-134">String collection</span></span>|<span data-ttu-id="0d95a-135">Office の構成のポリシー id のリスト</span><span class="sxs-lookup"><span data-stu-id="0d95a-135">List of office configuration policy ids</span></span>|
|<span data-ttu-id="0d95a-136">officeConfigurationPriorities</span><span class="sxs-lookup"><span data-stu-id="0d95a-136">officeConfigurationPriorities</span></span>|<span data-ttu-id="0d95a-137">Int32 型のコレクション</span><span class="sxs-lookup"><span data-stu-id="0d95a-137">Int32 collection</span></span>|<span data-ttu-id="0d95a-138">Office 設定の優先順位の一覧</span><span class="sxs-lookup"><span data-stu-id="0d95a-138">List of office configuration priorities</span></span>|



## <a name="response"></a><span data-ttu-id="0d95a-139">応答</span><span class="sxs-lookup"><span data-stu-id="0d95a-139">Response</span></span>
<span data-ttu-id="0d95a-140">成功した場合、このアクションは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="0d95a-140">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0d95a-141">例</span><span class="sxs-lookup"><span data-stu-id="0d95a-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="0d95a-142">要求</span><span class="sxs-lookup"><span data-stu-id="0d95a-142">Request</span></span>
<span data-ttu-id="0d95a-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0d95a-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0d95a-144">応答</span><span class="sxs-lookup"><span data-stu-id="0d95a-144">Response</span></span>
<span data-ttu-id="0d95a-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0d95a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```



