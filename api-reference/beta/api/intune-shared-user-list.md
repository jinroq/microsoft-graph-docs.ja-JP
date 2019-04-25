---
title: ユーザーを一覧表示する
description: user オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2ebdc1842eb3530a0327326b2c06fa87eb92563a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526910"
---
# <a name="list-users"></a><span data-ttu-id="16113-103">ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="16113-103">List users</span></span>

> <span data-ttu-id="16113-104">**重要:** Microsoft Graph の/ベータ版の api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="16113-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="16113-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16113-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16113-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="16113-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16113-107">[user](../resources/intune-shared-user.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="16113-107">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16113-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="16113-108">Prerequisites</span></span>

<span data-ttu-id="16113-109">この API を呼び出すには、次のいずれかのアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="16113-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="16113-110">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="16113-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="16113-111">特定のアクセス許可は、コンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="16113-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="16113-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="16113-112">Permission type</span></span>|<span data-ttu-id="16113-113">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="16113-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16113-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="16113-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="16113-115">&nbsp;&nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="16113-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="16113-116">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="16113-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="16113-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="16113-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="16113-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="16113-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="16113-119">&nbsp; &nbsp; **オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="16113-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="16113-120">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="16113-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="16113-121">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="16113-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="16113-122">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="16113-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="16113-123">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="16113-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16113-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16113-124">Not supported.</span></span>|
|<span data-ttu-id="16113-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="16113-125">Application</span></span>|<span data-ttu-id="16113-126">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16113-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16113-127">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="16113-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="16113-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16113-128">Request headers</span></span>

|<span data-ttu-id="16113-129">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16113-129">Header</span></span>|<span data-ttu-id="16113-130">値</span><span class="sxs-lookup"><span data-stu-id="16113-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16113-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="16113-131">Authorization</span></span>|<span data-ttu-id="16113-132">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="16113-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16113-133">承諾</span><span class="sxs-lookup"><span data-stu-id="16113-133">Accept</span></span>|<span data-ttu-id="16113-134">application/json</span><span class="sxs-lookup"><span data-stu-id="16113-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16113-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="16113-135">Request body</span></span>

<span data-ttu-id="16113-136">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="16113-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16113-137">応答</span><span class="sxs-lookup"><span data-stu-id="16113-137">Response</span></span>

<span data-ttu-id="16113-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [user](../resources/intune-shared-user.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="16113-138">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16113-139">例</span><span class="sxs-lookup"><span data-stu-id="16113-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="16113-140">要求</span><span class="sxs-lookup"><span data-stu-id="16113-140">Request</span></span>

<span data-ttu-id="16113-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="16113-141">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users
```

### <a name="response"></a><span data-ttu-id="16113-142">応答</span><span class="sxs-lookup"><span data-stu-id="16113-142">Response</span></span>

<span data-ttu-id="16113-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="16113-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 136

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
    }
  ]
}
```



