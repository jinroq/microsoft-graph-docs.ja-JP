---
title: removeAllDevicesFromManagement アクション
description: 対象ユーザーの管理からすべてのデバイスを破棄します
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d35b852ef9694a2e9d8f427ba3bbb98cb2b4c26a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025765"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="43b21-103">removeAllDevicesFromManagement アクション</span><span class="sxs-lookup"><span data-stu-id="43b21-103">removeAllDevicesFromManagement action</span></span>

> <span data-ttu-id="43b21-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="43b21-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43b21-105">対象ユーザーの管理からすべてのデバイスを破棄します</span><span class="sxs-lookup"><span data-stu-id="43b21-105">Retire all devices from management for this user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43b21-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="43b21-106">Prerequisites</span></span>
<span data-ttu-id="43b21-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="43b21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43b21-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="43b21-109">Permission type</span></span>|<span data-ttu-id="43b21-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="43b21-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43b21-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="43b21-111">Delegated (work or school account)</span></span>| <span data-ttu-id="43b21-112">_コンテキストによって異なる_</span><span class="sxs-lookup"><span data-stu-id="43b21-112">_varies by context_</span></span> |
| <span data-ttu-id="43b21-113">&nbsp;&nbsp;デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="43b21-113">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="43b21-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="43b21-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span> |
|<span data-ttu-id="43b21-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="43b21-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43b21-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43b21-116">Not supported.</span></span>|
|<span data-ttu-id="43b21-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="43b21-117">Application</span></span>|<span data-ttu-id="43b21-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43b21-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43b21-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="43b21-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="43b21-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="43b21-120">Request headers</span></span>
|<span data-ttu-id="43b21-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="43b21-121">Header</span></span>|<span data-ttu-id="43b21-122">値</span><span class="sxs-lookup"><span data-stu-id="43b21-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43b21-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="43b21-123">Authorization</span></span>|<span data-ttu-id="43b21-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="43b21-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43b21-125">承諾</span><span class="sxs-lookup"><span data-stu-id="43b21-125">Accept</span></span>|<span data-ttu-id="43b21-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43b21-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43b21-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="43b21-127">Request body</span></span>
<span data-ttu-id="43b21-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="43b21-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43b21-129">応答</span><span class="sxs-lookup"><span data-stu-id="43b21-129">Response</span></span>
<span data-ttu-id="43b21-130">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="43b21-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="43b21-131">例</span><span class="sxs-lookup"><span data-stu-id="43b21-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="43b21-132">要求</span><span class="sxs-lookup"><span data-stu-id="43b21-132">Request</span></span>
<span data-ttu-id="43b21-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="43b21-133">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="43b21-134">応答</span><span class="sxs-lookup"><span data-stu-id="43b21-134">Response</span></span>
<span data-ttu-id="43b21-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="43b21-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



