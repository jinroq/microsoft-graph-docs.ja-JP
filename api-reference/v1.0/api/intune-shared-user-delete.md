---
title: ユーザーを削除する
description: user を削除します。
author: tfitzmac
ms.openlocfilehash: 8ed00b2967fa04fd23351c7dbc369b25d97cba39
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337318"
---
# <a name="delete-user"></a><span data-ttu-id="698ff-103">ユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="698ff-103">Delete user</span></span>

> <span data-ttu-id="698ff-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="698ff-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="698ff-105">[user](../resources/intune-shared-user.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="698ff-105">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="698ff-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="698ff-106">Prerequisites</span></span>
<span data-ttu-id="698ff-107">この API を呼び出すには次のアクセス許可のいずれかが必要です。</span><span class="sxs-lookup"><span data-stu-id="698ff-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="698ff-108">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="698ff-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="698ff-109">必要な特定のアクセス許可は、コンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="698ff-109">The specific permission required depends on context.</span></span>

|<span data-ttu-id="698ff-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="698ff-110">Permission type</span></span>|<span data-ttu-id="698ff-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="698ff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="698ff-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="698ff-112">Delegated (work or school account)</span></span>| <span data-ttu-id="698ff-113">_コンテキストによって異なります_</span><span class="sxs-lookup"><span data-stu-id="698ff-113">_varies by context_</span></span>|
| <span data-ttu-id="698ff-114">&nbsp;&nbsp;デバイス</span><span class="sxs-lookup"><span data-stu-id="698ff-114">&nbsp; &nbsp; Devices</span></span> | <span data-ttu-id="698ff-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="698ff-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="698ff-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="698ff-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="698ff-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="698ff-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="698ff-118">&nbsp;&nbsp;契約時</span><span class="sxs-lookup"><span data-stu-id="698ff-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="698ff-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="698ff-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="698ff-120">&nbsp;&nbsp;のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="698ff-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="698ff-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="698ff-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="698ff-122">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="698ff-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="698ff-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="698ff-123">Not supported.</span></span>|
|<span data-ttu-id="698ff-124">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="698ff-124">Application</span></span>|<span data-ttu-id="698ff-125">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="698ff-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="698ff-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="698ff-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="698ff-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="698ff-127">Request headers</span></span>
|<span data-ttu-id="698ff-128">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="698ff-128">Header</span></span>|<span data-ttu-id="698ff-129">値</span><span class="sxs-lookup"><span data-stu-id="698ff-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="698ff-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="698ff-130">Authorization</span></span>|<span data-ttu-id="698ff-131">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="698ff-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="698ff-132">Accept</span><span class="sxs-lookup"><span data-stu-id="698ff-132">Accept</span></span>|<span data-ttu-id="698ff-133">application/json</span><span class="sxs-lookup"><span data-stu-id="698ff-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="698ff-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="698ff-134">Request body</span></span>
<span data-ttu-id="698ff-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="698ff-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="698ff-136">応答</span><span class="sxs-lookup"><span data-stu-id="698ff-136">Response</span></span>
<span data-ttu-id="698ff-137">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="698ff-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="698ff-138">例</span><span class="sxs-lookup"><span data-stu-id="698ff-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="698ff-139">要求</span><span class="sxs-lookup"><span data-stu-id="698ff-139">Request</span></span>
<span data-ttu-id="698ff-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="698ff-140">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="698ff-141">応答</span><span class="sxs-lookup"><span data-stu-id="698ff-141">Response</span></span>
<span data-ttu-id="698ff-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="698ff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



