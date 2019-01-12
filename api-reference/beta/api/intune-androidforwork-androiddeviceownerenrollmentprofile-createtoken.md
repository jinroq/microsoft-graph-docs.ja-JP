---
title: createToken アクション
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1ca3af2577e6b912b4389a9b2580a33a2063fe0d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945966"
---
# <a name="createtoken-action"></a><span data-ttu-id="74534-103">createToken アクション</span><span class="sxs-lookup"><span data-stu-id="74534-103">createToken action</span></span>

> <span data-ttu-id="74534-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="74534-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74534-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74534-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="74534-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="74534-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74534-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="74534-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="74534-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="74534-108">Prerequisites</span></span>
<span data-ttu-id="74534-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74534-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74534-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="74534-111">Permission type</span></span>|<span data-ttu-id="74534-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="74534-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74534-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="74534-113">Delegated (work or school account)</span></span>|<span data-ttu-id="74534-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74534-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="74534-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="74534-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74534-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74534-116">Not supported.</span></span>|
|<span data-ttu-id="74534-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="74534-117">Application</span></span>|<span data-ttu-id="74534-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74534-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74534-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="74534-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}/createToken
```

## <a name="request-headers"></a><span data-ttu-id="74534-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="74534-120">Request headers</span></span>
|<span data-ttu-id="74534-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="74534-121">Header</span></span>|<span data-ttu-id="74534-122">値</span><span class="sxs-lookup"><span data-stu-id="74534-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74534-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="74534-123">Authorization</span></span>|<span data-ttu-id="74534-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="74534-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74534-125">Accept</span><span class="sxs-lookup"><span data-stu-id="74534-125">Accept</span></span>|<span data-ttu-id="74534-126">application/json</span><span class="sxs-lookup"><span data-stu-id="74534-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74534-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="74534-127">Request body</span></span>
<span data-ttu-id="74534-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="74534-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="74534-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="74534-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="74534-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="74534-130">Property</span></span>|<span data-ttu-id="74534-131">種類</span><span class="sxs-lookup"><span data-stu-id="74534-131">Type</span></span>|<span data-ttu-id="74534-132">説明</span><span class="sxs-lookup"><span data-stu-id="74534-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74534-133">tokenValidityInSeconds</span><span class="sxs-lookup"><span data-stu-id="74534-133">tokenValidityInSeconds</span></span>|<span data-ttu-id="74534-134">Int32</span><span class="sxs-lookup"><span data-stu-id="74534-134">Int32</span></span>|<span data-ttu-id="74534-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="74534-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="74534-136">応答</span><span class="sxs-lookup"><span data-stu-id="74534-136">Response</span></span>
<span data-ttu-id="74534-137">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="74534-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="74534-138">例</span><span class="sxs-lookup"><span data-stu-id="74534-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="74534-139">要求</span><span class="sxs-lookup"><span data-stu-id="74534-139">Request</span></span>
<span data-ttu-id="74534-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="74534-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}/createToken

Content-type: application/json
Content-length: 35

{
  "tokenValidityInSeconds": 6
}
```

### <a name="response"></a><span data-ttu-id="74534-141">応答</span><span class="sxs-lookup"><span data-stu-id="74534-141">Response</span></span>
<span data-ttu-id="74534-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="74534-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





