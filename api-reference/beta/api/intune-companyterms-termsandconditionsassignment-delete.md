---
title: termsAndConditionsAssignment の削除
description: termsAndConditionsAssignment を削除します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a548367fd6d37ebe1f58150d53abeb90cf6f6369
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960939"
---
# <a name="delete-termsandconditionsassignment"></a><span data-ttu-id="b28f2-103">termsAndConditionsAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="b28f2-103">Delete termsAndConditionsAssignment</span></span>

> <span data-ttu-id="b28f2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b28f2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b28f2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b28f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b28f2-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b28f2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b28f2-107">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="b28f2-107">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b28f2-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b28f2-108">Prerequisites</span></span>
<span data-ttu-id="b28f2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b28f2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b28f2-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b28f2-111">Permission type</span></span>|<span data-ttu-id="b28f2-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b28f2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b28f2-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b28f2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b28f2-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b28f2-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b28f2-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b28f2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b28f2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b28f2-116">Not supported.</span></span>|
|<span data-ttu-id="b28f2-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b28f2-117">Application</span></span>|<span data-ttu-id="b28f2-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b28f2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b28f2-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b28f2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b28f2-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b28f2-120">Request headers</span></span>
|<span data-ttu-id="b28f2-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b28f2-121">Header</span></span>|<span data-ttu-id="b28f2-122">値</span><span class="sxs-lookup"><span data-stu-id="b28f2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b28f2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b28f2-123">Authorization</span></span>|<span data-ttu-id="b28f2-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b28f2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b28f2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b28f2-125">Accept</span></span>|<span data-ttu-id="b28f2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b28f2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b28f2-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b28f2-127">Request body</span></span>
<span data-ttu-id="b28f2-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b28f2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b28f2-129">応答</span><span class="sxs-lookup"><span data-stu-id="b28f2-129">Response</span></span>
<span data-ttu-id="b28f2-130">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="b28f2-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b28f2-131">例</span><span class="sxs-lookup"><span data-stu-id="b28f2-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b28f2-132">要求</span><span class="sxs-lookup"><span data-stu-id="b28f2-132">Request</span></span>
<span data-ttu-id="b28f2-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b28f2-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

### <a name="response"></a><span data-ttu-id="b28f2-134">応答</span><span class="sxs-lookup"><span data-stu-id="b28f2-134">Response</span></span>
<span data-ttu-id="b28f2-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b28f2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





