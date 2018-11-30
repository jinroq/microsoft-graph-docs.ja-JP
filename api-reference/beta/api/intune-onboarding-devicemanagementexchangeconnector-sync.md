---
title: sync アクション
description: まだ文書化されていません
ms.openlocfilehash: 6f3e1101537ff3b49d1a4c3e7933f78f2e11cbe3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074531"
---
# <a name="sync-action"></a><span data-ttu-id="925ad-103">sync アクション</span><span class="sxs-lookup"><span data-stu-id="925ad-103">sync action</span></span>

> <span data-ttu-id="925ad-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="925ad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="925ad-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="925ad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="925ad-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="925ad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="925ad-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="925ad-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="925ad-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="925ad-108">Prerequisites</span></span>
<span data-ttu-id="925ad-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="925ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="925ad-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="925ad-111">Permission type</span></span>|<span data-ttu-id="925ad-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="925ad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="925ad-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="925ad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="925ad-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="925ad-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="925ad-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="925ad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="925ad-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="925ad-116">Not supported.</span></span>|
|<span data-ttu-id="925ad-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="925ad-117">Application</span></span>|<span data-ttu-id="925ad-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="925ad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="925ad-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="925ad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync
```

## <a name="request-headers"></a><span data-ttu-id="925ad-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="925ad-120">Request headers</span></span>
|<span data-ttu-id="925ad-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="925ad-121">Header</span></span>|<span data-ttu-id="925ad-122">値</span><span class="sxs-lookup"><span data-stu-id="925ad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="925ad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="925ad-123">Authorization</span></span>|<span data-ttu-id="925ad-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="925ad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="925ad-125">Accept</span><span class="sxs-lookup"><span data-stu-id="925ad-125">Accept</span></span>|<span data-ttu-id="925ad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="925ad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="925ad-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="925ad-127">Request body</span></span>
<span data-ttu-id="925ad-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="925ad-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="925ad-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="925ad-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="925ad-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="925ad-130">Property</span></span>|<span data-ttu-id="925ad-131">型</span><span class="sxs-lookup"><span data-stu-id="925ad-131">Type</span></span>|<span data-ttu-id="925ad-132">説明</span><span class="sxs-lookup"><span data-stu-id="925ad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="925ad-133">syncType</span><span class="sxs-lookup"><span data-stu-id="925ad-133">syncType</span></span>|[<span data-ttu-id="925ad-134">deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="925ad-134">deviceManagementExchangeConnectorSyncType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorsynctype.md)|<span data-ttu-id="925ad-135">実行される同期の種類。完全同期またはデルタ同期のどちらかです。</span><span class="sxs-lookup"><span data-stu-id="925ad-135">The type of sync which will be executed, full sync or delta sync.</span></span>|



## <a name="response"></a><span data-ttu-id="925ad-136">応答</span><span class="sxs-lookup"><span data-stu-id="925ad-136">Response</span></span>
<span data-ttu-id="925ad-137">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="925ad-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="925ad-138">例</span><span class="sxs-lookup"><span data-stu-id="925ad-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="925ad-139">要求</span><span class="sxs-lookup"><span data-stu-id="925ad-139">Request</span></span>
<span data-ttu-id="925ad-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="925ad-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync

Content-type: application/json
Content-length: 31

{
  "syncType": "deltaSync"
}
```

### <a name="response"></a><span data-ttu-id="925ad-141">応答</span><span class="sxs-lookup"><span data-stu-id="925ad-141">Response</span></span>
<span data-ttu-id="925ad-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="925ad-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





