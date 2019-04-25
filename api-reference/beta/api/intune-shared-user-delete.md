---
title: ユーザーを削除する
description: user を削除します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ecf07bf080a76e6f1fce515d41090be214e7a514
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526861"
---
# <a name="delete-user"></a><span data-ttu-id="13f50-103">ユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="13f50-103">Delete user</span></span>

> <span data-ttu-id="13f50-104">**重要:** Microsoft Graph の/ベータ版の api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="13f50-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="13f50-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13f50-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="13f50-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="13f50-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13f50-107">[user](../resources/intune-shared-user.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="13f50-107">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="13f50-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="13f50-108">Prerequisites</span></span>
<span data-ttu-id="13f50-109">この API を呼び出すには、次のいずれかのアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="13f50-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="13f50-110">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="13f50-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="13f50-111">必要な特定のアクセス許可は、コンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="13f50-111">The specific permission required depends on context.</span></span>

|<span data-ttu-id="13f50-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="13f50-112">Permission type</span></span>|<span data-ttu-id="13f50-113">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="13f50-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13f50-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="13f50-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="13f50-115">&nbsp;&nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="13f50-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="13f50-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13f50-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="13f50-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="13f50-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="13f50-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13f50-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="13f50-119">&nbsp; &nbsp; **オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="13f50-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="13f50-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13f50-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="13f50-121">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="13f50-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="13f50-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13f50-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="13f50-123">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="13f50-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13f50-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13f50-124">Not supported.</span></span>|
|<span data-ttu-id="13f50-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="13f50-125">Application</span></span>|<span data-ttu-id="13f50-126">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13f50-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13f50-127">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="13f50-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="13f50-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13f50-128">Request headers</span></span>

|<span data-ttu-id="13f50-129">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13f50-129">Header</span></span>|<span data-ttu-id="13f50-130">値</span><span class="sxs-lookup"><span data-stu-id="13f50-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13f50-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="13f50-131">Authorization</span></span>|<span data-ttu-id="13f50-132">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="13f50-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13f50-133">承諾</span><span class="sxs-lookup"><span data-stu-id="13f50-133">Accept</span></span>|<span data-ttu-id="13f50-134">application/json</span><span class="sxs-lookup"><span data-stu-id="13f50-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13f50-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="13f50-135">Request body</span></span>

<span data-ttu-id="13f50-136">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="13f50-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13f50-137">応答</span><span class="sxs-lookup"><span data-stu-id="13f50-137">Response</span></span>

<span data-ttu-id="13f50-138">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="13f50-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="13f50-139">例</span><span class="sxs-lookup"><span data-stu-id="13f50-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="13f50-140">要求</span><span class="sxs-lookup"><span data-stu-id="13f50-140">Request</span></span>

<span data-ttu-id="13f50-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="13f50-141">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="13f50-142">応答</span><span class="sxs-lookup"><span data-stu-id="13f50-142">Response</span></span>

<span data-ttu-id="13f50-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="13f50-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



