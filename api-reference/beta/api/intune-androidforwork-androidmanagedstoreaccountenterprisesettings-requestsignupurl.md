---
title: requestSignupUrl アクション
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5eab1e241eddbcb4ac49002b8ae411932dee4b1b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921928"
---
# <a name="requestsignupurl-action"></a><span data-ttu-id="9e390-103">requestSignupUrl アクション</span><span class="sxs-lookup"><span data-stu-id="9e390-103">requestSignupUrl action</span></span>

> <span data-ttu-id="9e390-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9e390-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e390-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e390-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9e390-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9e390-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e390-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9e390-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9e390-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9e390-108">Prerequisites</span></span>
<span data-ttu-id="9e390-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9e390-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e390-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9e390-111">Permission type</span></span>|<span data-ttu-id="9e390-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9e390-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e390-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9e390-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9e390-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e390-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9e390-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9e390-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e390-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e390-116">Not supported.</span></span>|
|<span data-ttu-id="9e390-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9e390-117">Application</span></span>|<span data-ttu-id="9e390-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e390-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e390-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9e390-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/requestSignupUrl
```

## <a name="request-headers"></a><span data-ttu-id="9e390-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e390-120">Request headers</span></span>
|<span data-ttu-id="9e390-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e390-121">Header</span></span>|<span data-ttu-id="9e390-122">値</span><span class="sxs-lookup"><span data-stu-id="9e390-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e390-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e390-123">Authorization</span></span>|<span data-ttu-id="9e390-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9e390-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e390-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9e390-125">Accept</span></span>|<span data-ttu-id="9e390-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9e390-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e390-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9e390-127">Request body</span></span>
<span data-ttu-id="9e390-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9e390-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9e390-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="9e390-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9e390-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e390-130">Property</span></span>|<span data-ttu-id="9e390-131">型</span><span class="sxs-lookup"><span data-stu-id="9e390-131">Type</span></span>|<span data-ttu-id="9e390-132">説明</span><span class="sxs-lookup"><span data-stu-id="9e390-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e390-133">hostName</span><span class="sxs-lookup"><span data-stu-id="9e390-133">hostName</span></span>|<span data-ttu-id="9e390-134">String</span><span class="sxs-lookup"><span data-stu-id="9e390-134">String</span></span>|<span data-ttu-id="9e390-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9e390-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9e390-136">応答</span><span class="sxs-lookup"><span data-stu-id="9e390-136">Response</span></span>
<span data-ttu-id="9e390-137">成功した場合、この関数は `200 OK` 応答コードと、応答本文で String を返します。</span><span class="sxs-lookup"><span data-stu-id="9e390-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e390-138">例</span><span class="sxs-lookup"><span data-stu-id="9e390-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="9e390-139">要求</span><span class="sxs-lookup"><span data-stu-id="9e390-139">Request</span></span>
<span data-ttu-id="9e390-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9e390-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/requestSignupUrl

Content-type: application/json
Content-length: 37

{
  "hostName": "Host Name value"
}
```

### <a name="response"></a><span data-ttu-id="9e390-141">応答</span><span class="sxs-lookup"><span data-stu-id="9e390-141">Response</span></span>
<span data-ttu-id="9e390-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9e390-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 56

{
  "value": "https://example.com/requestSignupUrl/"
}
```





