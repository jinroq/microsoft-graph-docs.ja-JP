---
title: SideLoadingKey を削除します。
description: SideLoadingKey を削除します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d3cfe967643c9c5cd2c269d96b7b6edd09fd55a7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971061"
---
# <a name="delete-sideloadingkey"></a><span data-ttu-id="7e833-103">SideLoadingKey を削除します。</span><span class="sxs-lookup"><span data-stu-id="7e833-103">Delete sideLoadingKey</span></span>

> <span data-ttu-id="7e833-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7e833-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7e833-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e833-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7e833-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7e833-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e833-107">の[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="7e833-107">Deletes a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7e833-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7e833-108">Prerequisites</span></span>
<span data-ttu-id="7e833-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7e833-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e833-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7e833-111">Permission type</span></span>|<span data-ttu-id="7e833-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7e833-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e833-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7e833-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7e833-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e833-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7e833-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7e833-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e833-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e833-116">Not supported.</span></span>|
|<span data-ttu-id="7e833-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7e833-117">Application</span></span>|<span data-ttu-id="7e833-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e833-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e833-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7e833-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

## <a name="request-headers"></a><span data-ttu-id="7e833-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7e833-120">Request headers</span></span>
|<span data-ttu-id="7e833-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7e833-121">Header</span></span>|<span data-ttu-id="7e833-122">値</span><span class="sxs-lookup"><span data-stu-id="7e833-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e833-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e833-123">Authorization</span></span>|<span data-ttu-id="7e833-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7e833-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e833-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7e833-125">Accept</span></span>|<span data-ttu-id="7e833-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7e833-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e833-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7e833-127">Request body</span></span>
<span data-ttu-id="7e833-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7e833-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e833-129">応答</span><span class="sxs-lookup"><span data-stu-id="7e833-129">Response</span></span>
<span data-ttu-id="7e833-130">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="7e833-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7e833-131">例</span><span class="sxs-lookup"><span data-stu-id="7e833-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="7e833-132">要求</span><span class="sxs-lookup"><span data-stu-id="7e833-132">Request</span></span>
<span data-ttu-id="7e833-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7e833-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

### <a name="response"></a><span data-ttu-id="7e833-134">応答</span><span class="sxs-lookup"><span data-stu-id="7e833-134">Response</span></span>
<span data-ttu-id="7e833-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7e833-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





