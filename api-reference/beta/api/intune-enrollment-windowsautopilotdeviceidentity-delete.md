---
title: WindowsAutopilotDeviceIdentity を削除します。
description: WindowsAutopilotDeviceIdentity を削除します。
author: tfitzmac
ms.openlocfilehash: 5194536ef6526714819ee676ef063997b1a39895
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304278"
---
# <a name="delete-windowsautopilotdeviceidentity"></a><span data-ttu-id="04b72-103">WindowsAutopilotDeviceIdentity を削除します。</span><span class="sxs-lookup"><span data-stu-id="04b72-103">Delete windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="04b72-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="04b72-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04b72-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04b72-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04b72-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="04b72-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04b72-107">の[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="04b72-107">Deletes a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="04b72-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="04b72-108">Prerequisites</span></span>
<span data-ttu-id="04b72-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04b72-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04b72-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="04b72-111">Permission type</span></span>|<span data-ttu-id="04b72-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="04b72-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04b72-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="04b72-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04b72-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04b72-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="04b72-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="04b72-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04b72-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04b72-116">Not supported.</span></span>|
|<span data-ttu-id="04b72-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="04b72-117">Application</span></span>|<span data-ttu-id="04b72-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04b72-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04b72-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="04b72-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
DELETE /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="04b72-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04b72-120">Request headers</span></span>
|<span data-ttu-id="04b72-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04b72-121">Header</span></span>|<span data-ttu-id="04b72-122">値</span><span class="sxs-lookup"><span data-stu-id="04b72-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04b72-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="04b72-123">Authorization</span></span>|<span data-ttu-id="04b72-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="04b72-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04b72-125">Accept</span><span class="sxs-lookup"><span data-stu-id="04b72-125">Accept</span></span>|<span data-ttu-id="04b72-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04b72-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04b72-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="04b72-127">Request body</span></span>
<span data-ttu-id="04b72-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="04b72-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04b72-129">応答</span><span class="sxs-lookup"><span data-stu-id="04b72-129">Response</span></span>
<span data-ttu-id="04b72-130">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="04b72-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="04b72-131">例</span><span class="sxs-lookup"><span data-stu-id="04b72-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="04b72-132">要求</span><span class="sxs-lookup"><span data-stu-id="04b72-132">Request</span></span>
<span data-ttu-id="04b72-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="04b72-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="04b72-134">応答</span><span class="sxs-lookup"><span data-stu-id="04b72-134">Response</span></span>
<span data-ttu-id="04b72-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="04b72-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





