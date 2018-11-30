---
title: createGooglePlayWebToken アクション
description: 組み込み可能なコンポーネントで使用される web トークンを生成します。
ms.openlocfilehash: 26b58e5973063a74cac69d0bb70aa02adde7093f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071749"
---
# <a name="creategoogleplaywebtoken-action"></a><span data-ttu-id="98719-103">createGooglePlayWebToken アクション</span><span class="sxs-lookup"><span data-stu-id="98719-103">createGooglePlayWebToken action</span></span>

> <span data-ttu-id="98719-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="98719-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98719-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="98719-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="98719-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="98719-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98719-107">組み込み可能なコンポーネントで使用される web トークンを生成します。</span><span class="sxs-lookup"><span data-stu-id="98719-107">Generates a web token that is used in an embeddable component.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="98719-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="98719-108">Prerequisites</span></span>
<span data-ttu-id="98719-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="98719-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98719-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="98719-111">Permission type</span></span>|<span data-ttu-id="98719-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="98719-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98719-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="98719-113">Delegated (work or school account)</span></span>|<span data-ttu-id="98719-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98719-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="98719-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="98719-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98719-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="98719-116">Not supported.</span></span>|
|<span data-ttu-id="98719-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="98719-117">Application</span></span>|<span data-ttu-id="98719-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="98719-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98719-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="98719-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken
```

## <a name="request-headers"></a><span data-ttu-id="98719-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="98719-120">Request headers</span></span>
|<span data-ttu-id="98719-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="98719-121">Header</span></span>|<span data-ttu-id="98719-122">値</span><span class="sxs-lookup"><span data-stu-id="98719-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98719-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="98719-123">Authorization</span></span>|<span data-ttu-id="98719-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="98719-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98719-125">Accept</span><span class="sxs-lookup"><span data-stu-id="98719-125">Accept</span></span>|<span data-ttu-id="98719-126">application/json</span><span class="sxs-lookup"><span data-stu-id="98719-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98719-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="98719-127">Request body</span></span>
<span data-ttu-id="98719-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="98719-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="98719-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="98719-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="98719-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="98719-130">Property</span></span>|<span data-ttu-id="98719-131">型</span><span class="sxs-lookup"><span data-stu-id="98719-131">Type</span></span>|<span data-ttu-id="98719-132">説明</span><span class="sxs-lookup"><span data-stu-id="98719-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98719-133">parentUri</span><span class="sxs-lookup"><span data-stu-id="98719-133">parentUri</span></span>|<span data-ttu-id="98719-134">String</span><span class="sxs-lookup"><span data-stu-id="98719-134">String</span></span>|<span data-ttu-id="98719-135">Https のコンポーネントをホストしているページのパス。</span><span class="sxs-lookup"><span data-stu-id="98719-135">The https path of the page hosting the component.</span></span>|



## <a name="response"></a><span data-ttu-id="98719-136">応答</span><span class="sxs-lookup"><span data-stu-id="98719-136">Response</span></span>
<span data-ttu-id="98719-137">成功した場合、この関数は `200 OK` 応答コードと、応答本文で String を返します。</span><span class="sxs-lookup"><span data-stu-id="98719-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98719-138">例</span><span class="sxs-lookup"><span data-stu-id="98719-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="98719-139">要求</span><span class="sxs-lookup"><span data-stu-id="98719-139">Request</span></span>
<span data-ttu-id="98719-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="98719-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken

Content-type: application/json
Content-length: 39

{
  "parentUri": "Parent Uri value"
}
```

### <a name="response"></a><span data-ttu-id="98719-141">応答</span><span class="sxs-lookup"><span data-stu-id="98719-141">Response</span></span>
<span data-ttu-id="98719-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="98719-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 53

{
  "value": "Create Google Play Web Token value"
}
```





