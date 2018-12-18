---
title: ユーザーを取得する
description: user オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
ms.openlocfilehash: b58485112929f39be76f1f908f3097d8971ac564
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303305"
---
# <a name="get-user"></a><span data-ttu-id="48401-103">ユーザーを取得する</span><span class="sxs-lookup"><span data-stu-id="48401-103">Get user</span></span>

> <span data-ttu-id="48401-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="48401-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="48401-105">[user](../resources/intune-shared-user.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="48401-105">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="48401-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="48401-106">Prerequisites</span></span>
<span data-ttu-id="48401-107">この API を呼び出すには次のアクセス許可のいずれかが必要です。</span><span class="sxs-lookup"><span data-stu-id="48401-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="48401-108">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="48401-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="48401-109">特定のアクセス許可は、コンテキストに依存します。</span><span class="sxs-lookup"><span data-stu-id="48401-109">The specific permission depends on the context.</span></span>

|<span data-ttu-id="48401-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="48401-110">Permission type</span></span>|<span data-ttu-id="48401-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="48401-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48401-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="48401-112">Delegated (work or school account)</span></span>| <span data-ttu-id="48401-113">_コンテキストによって異なります_</span><span class="sxs-lookup"><span data-stu-id="48401-113">_varies by context_</span></span>|
| <span data-ttu-id="48401-114">&nbsp;&nbsp;デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="48401-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="48401-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="48401-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="48401-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="48401-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="48401-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="48401-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="48401-118">&nbsp;&nbsp;契約時</span><span class="sxs-lookup"><span data-stu-id="48401-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="48401-119">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="48401-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="48401-120">&nbsp;&nbsp;のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="48401-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="48401-121">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="48401-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="48401-122">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="48401-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48401-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48401-123">Not supported.</span></span>|
|<span data-ttu-id="48401-124">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="48401-124">Application</span></span>|<span data-ttu-id="48401-125">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48401-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48401-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="48401-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="48401-127">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="48401-127">Optional query parameters</span></span>
<span data-ttu-id="48401-128">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="48401-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="48401-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="48401-129">Request headers</span></span>
|<span data-ttu-id="48401-130">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="48401-130">Header</span></span>|<span data-ttu-id="48401-131">値</span><span class="sxs-lookup"><span data-stu-id="48401-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48401-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="48401-132">Authorization</span></span>|<span data-ttu-id="48401-133">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="48401-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48401-134">Accept</span><span class="sxs-lookup"><span data-stu-id="48401-134">Accept</span></span>|<span data-ttu-id="48401-135">application/json</span><span class="sxs-lookup"><span data-stu-id="48401-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48401-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="48401-136">Request body</span></span>
<span data-ttu-id="48401-137">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="48401-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48401-138">応答</span><span class="sxs-lookup"><span data-stu-id="48401-138">Response</span></span>
<span data-ttu-id="48401-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[ユーザー](../resources/intune-shared-user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="48401-139">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48401-140">例</span><span class="sxs-lookup"><span data-stu-id="48401-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="48401-141">要求</span><span class="sxs-lookup"><span data-stu-id="48401-141">Request</span></span>
<span data-ttu-id="48401-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="48401-142">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="48401-143">応答</span><span class="sxs-lookup"><span data-stu-id="48401-143">Response</span></span>
<span data-ttu-id="48401-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="48401-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 118

{
  "value": {
    "@odata.type": "#microsoft.graph.user",
    "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
  }
}
```



