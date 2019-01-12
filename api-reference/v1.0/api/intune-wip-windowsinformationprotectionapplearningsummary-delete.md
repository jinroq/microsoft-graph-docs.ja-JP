---
title: windowsInformationProtectionAppLearningSummary の削除
description: windowsInformationProtectionAppLearningSummary を削除します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0bf4b378f756e6f6c634484c24cdc396b734feef
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970774"
---
# <a name="delete-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="95728-103">windowsInformationProtectionAppLearningSummary の削除</span><span class="sxs-lookup"><span data-stu-id="95728-103">Delete windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="95728-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="95728-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="95728-105">[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="95728-105">Deletes a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="95728-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="95728-106">Prerequisites</span></span>
<span data-ttu-id="95728-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="95728-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95728-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="95728-109">Permission type</span></span>|<span data-ttu-id="95728-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="95728-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95728-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="95728-111">Delegated (work or school account)</span></span>|<span data-ttu-id="95728-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95728-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="95728-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="95728-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95728-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95728-114">Not supported.</span></span>|
|<span data-ttu-id="95728-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="95728-115">Application</span></span>|<span data-ttu-id="95728-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95728-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95728-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="95728-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="95728-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95728-118">Request headers</span></span>
|<span data-ttu-id="95728-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95728-119">Header</span></span>|<span data-ttu-id="95728-120">値</span><span class="sxs-lookup"><span data-stu-id="95728-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95728-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="95728-121">Authorization</span></span>|<span data-ttu-id="95728-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="95728-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95728-123">Accept</span><span class="sxs-lookup"><span data-stu-id="95728-123">Accept</span></span>|<span data-ttu-id="95728-124">application/json</span><span class="sxs-lookup"><span data-stu-id="95728-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95728-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="95728-125">Request body</span></span>
<span data-ttu-id="95728-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="95728-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95728-127">応答</span><span class="sxs-lookup"><span data-stu-id="95728-127">Response</span></span>
<span data-ttu-id="95728-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="95728-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="95728-129">例</span><span class="sxs-lookup"><span data-stu-id="95728-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="95728-130">要求</span><span class="sxs-lookup"><span data-stu-id="95728-130">Request</span></span>
<span data-ttu-id="95728-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="95728-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

### <a name="response"></a><span data-ttu-id="95728-132">応答</span><span class="sxs-lookup"><span data-stu-id="95728-132">Response</span></span>
<span data-ttu-id="95728-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="95728-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



