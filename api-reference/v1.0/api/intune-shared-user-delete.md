---
title: ユーザーを削除する
description: user を削除します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e66d987c2e88f40dd5b104961e9203dcd636651a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254626"
---
# <a name="delete-user"></a><span data-ttu-id="0acc0-103">ユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="0acc0-103">Delete user</span></span>

> <span data-ttu-id="0acc0-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0acc0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0acc0-105">[user](../resources/intune-shared-user.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="0acc0-105">Deletes a [user](../resources/intune-shared-user.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0acc0-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="0acc0-106">Prerequisites</span></span>
<span data-ttu-id="0acc0-107">この API を呼び出すには、次のいずれかのアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="0acc0-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="0acc0-108">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0acc0-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="0acc0-109">必要な特定のアクセス許可は、コンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="0acc0-109">The specific permission required depends on context.</span></span>

|<span data-ttu-id="0acc0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0acc0-110">Permission type</span></span>|<span data-ttu-id="0acc0-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0acc0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0acc0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0acc0-112">Delegated (work or school account)</span></span>| <span data-ttu-id="0acc0-113">_コンテキストによって異なる_</span><span class="sxs-lookup"><span data-stu-id="0acc0-113">_varies by context_</span></span>|
| <span data-ttu-id="0acc0-114">&nbsp;&nbsp;デバイス</span><span class="sxs-lookup"><span data-stu-id="0acc0-114">&nbsp; &nbsp; Devices</span></span> | <span data-ttu-id="0acc0-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0acc0-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="0acc0-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="0acc0-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="0acc0-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0acc0-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="0acc0-118">&nbsp;&nbsp;オンボード</span><span class="sxs-lookup"><span data-stu-id="0acc0-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="0acc0-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0acc0-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="0acc0-120">&nbsp;&nbsp;トラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="0acc0-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="0acc0-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0acc0-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="0acc0-122">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0acc0-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0acc0-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0acc0-123">Not supported.</span></span>|
|<span data-ttu-id="0acc0-124">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0acc0-124">Application</span></span>|<span data-ttu-id="0acc0-125">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0acc0-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0acc0-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0acc0-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="0acc0-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0acc0-127">Request headers</span></span>
|<span data-ttu-id="0acc0-128">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0acc0-128">Header</span></span>|<span data-ttu-id="0acc0-129">値</span><span class="sxs-lookup"><span data-stu-id="0acc0-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0acc0-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="0acc0-130">Authorization</span></span>|<span data-ttu-id="0acc0-131">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0acc0-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0acc0-132">承諾</span><span class="sxs-lookup"><span data-stu-id="0acc0-132">Accept</span></span>|<span data-ttu-id="0acc0-133">application/json</span><span class="sxs-lookup"><span data-stu-id="0acc0-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0acc0-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="0acc0-134">Request body</span></span>
<span data-ttu-id="0acc0-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0acc0-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0acc0-136">応答</span><span class="sxs-lookup"><span data-stu-id="0acc0-136">Response</span></span>
<span data-ttu-id="0acc0-137">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="0acc0-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0acc0-138">例</span><span class="sxs-lookup"><span data-stu-id="0acc0-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="0acc0-139">要求</span><span class="sxs-lookup"><span data-stu-id="0acc0-139">Request</span></span>
<span data-ttu-id="0acc0-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0acc0-140">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="0acc0-141">応答</span><span class="sxs-lookup"><span data-stu-id="0acc0-141">Response</span></span>
<span data-ttu-id="0acc0-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0acc0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



