---
title: removeAllDevicesFromManagement アクション
description: 対象ユーザーの管理からすべてのデバイスを破棄します
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dd2fd7e9794e816e40c6f844e24110e1ef1bcdaf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993495"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="54716-103">removeAllDevicesFromManagement アクション</span><span class="sxs-lookup"><span data-stu-id="54716-103">removeAllDevicesFromManagement action</span></span>

> <span data-ttu-id="54716-104">**重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="54716-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="54716-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54716-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="54716-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="54716-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54716-107">対象ユーザーの管理からすべてのデバイスを破棄します</span><span class="sxs-lookup"><span data-stu-id="54716-107">Retire all devices from management for this user</span></span>
## <a name="prerequisites"></a><span data-ttu-id="54716-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="54716-108">Prerequisites</span></span>
<span data-ttu-id="54716-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="54716-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54716-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="54716-111">Permission type</span></span>|<span data-ttu-id="54716-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="54716-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54716-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="54716-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="54716-114">&nbsp;&nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="54716-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="54716-115">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="54716-115">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="54716-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="54716-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54716-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54716-117">Not supported.</span></span>|
|<span data-ttu-id="54716-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="54716-118">Application</span></span>|<span data-ttu-id="54716-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54716-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54716-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="54716-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="54716-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="54716-121">Request headers</span></span>
|<span data-ttu-id="54716-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="54716-122">Header</span></span>|<span data-ttu-id="54716-123">値</span><span class="sxs-lookup"><span data-stu-id="54716-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54716-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="54716-124">Authorization</span></span>|<span data-ttu-id="54716-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="54716-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54716-126">承諾</span><span class="sxs-lookup"><span data-stu-id="54716-126">Accept</span></span>|<span data-ttu-id="54716-127">application/json</span><span class="sxs-lookup"><span data-stu-id="54716-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54716-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="54716-128">Request body</span></span>
<span data-ttu-id="54716-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="54716-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54716-130">応答</span><span class="sxs-lookup"><span data-stu-id="54716-130">Response</span></span>
<span data-ttu-id="54716-131">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="54716-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="54716-132">例</span><span class="sxs-lookup"><span data-stu-id="54716-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="54716-133">要求</span><span class="sxs-lookup"><span data-stu-id="54716-133">Request</span></span>
<span data-ttu-id="54716-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="54716-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="54716-135">応答</span><span class="sxs-lookup"><span data-stu-id="54716-135">Response</span></span>
<span data-ttu-id="54716-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="54716-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





