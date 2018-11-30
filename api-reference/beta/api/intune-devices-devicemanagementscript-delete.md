---
title: DeviceManagementScript を削除します。
description: DeviceManagementScript を削除します。
ms.openlocfilehash: bfbca0d626fcb46dc6a8a3b3cf32eaaed6818266
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069272"
---
# <a name="delete-devicemanagementscript"></a><span data-ttu-id="1f012-103">DeviceManagementScript を削除します。</span><span class="sxs-lookup"><span data-stu-id="1f012-103">Delete deviceManagementScript</span></span>

> <span data-ttu-id="1f012-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1f012-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f012-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f012-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1f012-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1f012-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f012-107">の[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="1f012-107">Deletes a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1f012-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="1f012-108">Prerequisites</span></span>
<span data-ttu-id="1f012-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1f012-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f012-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1f012-111">Permission type</span></span>|<span data-ttu-id="1f012-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1f012-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f012-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1f012-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1f012-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f012-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1f012-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1f012-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f012-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f012-116">Not supported.</span></span>|
|<span data-ttu-id="1f012-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1f012-117">Application</span></span>|<span data-ttu-id="1f012-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f012-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f012-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1f012-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="1f012-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1f012-120">Request headers</span></span>
|<span data-ttu-id="1f012-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1f012-121">Header</span></span>|<span data-ttu-id="1f012-122">値</span><span class="sxs-lookup"><span data-stu-id="1f012-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f012-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f012-123">Authorization</span></span>|<span data-ttu-id="1f012-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1f012-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f012-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1f012-125">Accept</span></span>|<span data-ttu-id="1f012-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1f012-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f012-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1f012-127">Request body</span></span>
<span data-ttu-id="1f012-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1f012-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f012-129">応答</span><span class="sxs-lookup"><span data-stu-id="1f012-129">Response</span></span>
<span data-ttu-id="1f012-130">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="1f012-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1f012-131">例</span><span class="sxs-lookup"><span data-stu-id="1f012-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="1f012-132">要求</span><span class="sxs-lookup"><span data-stu-id="1f012-132">Request</span></span>
<span data-ttu-id="1f012-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1f012-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

### <a name="response"></a><span data-ttu-id="1f012-134">応答</span><span class="sxs-lookup"><span data-stu-id="1f012-134">Response</span></span>
<span data-ttu-id="1f012-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1f012-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




