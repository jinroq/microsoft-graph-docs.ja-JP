---
title: removeAllDevicesFromManagement アクション
description: 対象ユーザーの管理からすべてのデバイスを破棄します
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 40baa470968c10bbe26af1d8397306f5b9e3f736
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576655"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="f66db-103">removeAllDevicesFromManagement アクション</span><span class="sxs-lookup"><span data-stu-id="f66db-103">removeAllDevicesFromManagement action</span></span>

> <span data-ttu-id="f66db-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f66db-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f66db-105">対象ユーザーの管理からすべてのデバイスを破棄します</span><span class="sxs-lookup"><span data-stu-id="f66db-105">Retire all devices from management for this user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f66db-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="f66db-106">Prerequisites</span></span>
<span data-ttu-id="f66db-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f66db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f66db-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f66db-109">Permission type</span></span>|<span data-ttu-id="f66db-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f66db-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f66db-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f66db-111">Delegated (work or school account)</span></span>| <span data-ttu-id="f66db-112">_コンテキストによって異なる_</span><span class="sxs-lookup"><span data-stu-id="f66db-112">_varies by context_</span></span> |
| <span data-ttu-id="f66db-113">&nbsp;&nbsp;デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="f66db-113">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="f66db-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="f66db-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span> |
|<span data-ttu-id="f66db-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f66db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f66db-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f66db-116">Not supported.</span></span>|
|<span data-ttu-id="f66db-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f66db-117">Application</span></span>|<span data-ttu-id="f66db-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f66db-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f66db-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f66db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="f66db-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f66db-120">Request headers</span></span>
|<span data-ttu-id="f66db-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f66db-121">Header</span></span>|<span data-ttu-id="f66db-122">値</span><span class="sxs-lookup"><span data-stu-id="f66db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f66db-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f66db-123">Authorization</span></span>|<span data-ttu-id="f66db-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f66db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f66db-125">承諾</span><span class="sxs-lookup"><span data-stu-id="f66db-125">Accept</span></span>|<span data-ttu-id="f66db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f66db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f66db-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f66db-127">Request body</span></span>
<span data-ttu-id="f66db-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f66db-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f66db-129">応答</span><span class="sxs-lookup"><span data-stu-id="f66db-129">Response</span></span>
<span data-ttu-id="f66db-130">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="f66db-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f66db-131">例</span><span class="sxs-lookup"><span data-stu-id="f66db-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f66db-132">要求</span><span class="sxs-lookup"><span data-stu-id="f66db-132">Request</span></span>
<span data-ttu-id="f66db-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f66db-133">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="f66db-134">応答</span><span class="sxs-lookup"><span data-stu-id="f66db-134">Response</span></span>
<span data-ttu-id="f66db-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f66db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



