---
title: Delete windowsInformationProtectionNetworkLearningSummary
description: windowsInformationProtectionNetworkLearningSummary を削除します。
ms.openlocfilehash: 098230894f1aa60becada7c301650034940d7e46
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069037"
---
# <a name="delete-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="80666-103">Delete windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="80666-103">Delete windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="80666-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="80666-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80666-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80666-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80666-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="80666-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80666-107">[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="80666-107">Deletes a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="80666-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="80666-108">Prerequisites</span></span>
<span data-ttu-id="80666-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="80666-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80666-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="80666-111">Permission type</span></span>|<span data-ttu-id="80666-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="80666-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80666-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="80666-113">Delegated (work or school account)</span></span>|<span data-ttu-id="80666-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80666-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="80666-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="80666-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80666-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80666-116">Not supported.</span></span>|
|<span data-ttu-id="80666-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="80666-117">Application</span></span>|<span data-ttu-id="80666-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80666-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80666-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="80666-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="80666-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="80666-120">Request headers</span></span>
|<span data-ttu-id="80666-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="80666-121">Header</span></span>|<span data-ttu-id="80666-122">値</span><span class="sxs-lookup"><span data-stu-id="80666-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80666-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="80666-123">Authorization</span></span>|<span data-ttu-id="80666-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="80666-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80666-125">Accept</span><span class="sxs-lookup"><span data-stu-id="80666-125">Accept</span></span>|<span data-ttu-id="80666-126">application/json</span><span class="sxs-lookup"><span data-stu-id="80666-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80666-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="80666-127">Request body</span></span>
<span data-ttu-id="80666-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="80666-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80666-129">応答</span><span class="sxs-lookup"><span data-stu-id="80666-129">Response</span></span>
<span data-ttu-id="80666-130">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="80666-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="80666-131">例</span><span class="sxs-lookup"><span data-stu-id="80666-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="80666-132">要求</span><span class="sxs-lookup"><span data-stu-id="80666-132">Request</span></span>
<span data-ttu-id="80666-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="80666-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

### <a name="response"></a><span data-ttu-id="80666-134">応答</span><span class="sxs-lookup"><span data-stu-id="80666-134">Response</span></span>
<span data-ttu-id="80666-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="80666-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




