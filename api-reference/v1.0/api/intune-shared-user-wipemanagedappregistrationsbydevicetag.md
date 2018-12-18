---
title: wipeManagedAppRegistrationsByDeviceTag アクション
description: 指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。
author: tfitzmac
ms.openlocfilehash: 227d702d217669215894c6e6c0cfd3fa67075277
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326384"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="7e3f9-103">wipeManagedAppRegistrationsByDeviceTag アクション</span><span class="sxs-lookup"><span data-stu-id="7e3f9-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>



> <span data-ttu-id="7e3f9-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7e3f9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e3f9-105">指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="7e3f9-105">Issues a wipe operation on an app registration with specified device tag.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7e3f9-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="7e3f9-106">Prerequisites</span></span>
<span data-ttu-id="7e3f9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7e3f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e3f9-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7e3f9-109">Permission type</span></span>|<span data-ttu-id="7e3f9-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7e3f9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e3f9-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7e3f9-111">Delegated (work or school account)</span></span>| <span data-ttu-id="7e3f9-112">_コンテキストによって異なります_</span><span class="sxs-lookup"><span data-stu-id="7e3f9-112">_varies by context_</span></span> |
| <span data-ttu-id="7e3f9-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="7e3f9-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="7e3f9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e3f9-114">DeviceManagementApps.ReadWrite.All</span></span> |
|<span data-ttu-id="7e3f9-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7e3f9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e3f9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e3f9-116">Not supported.</span></span>|
|<span data-ttu-id="7e3f9-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7e3f9-117">Application</span></span>|<span data-ttu-id="7e3f9-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e3f9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e3f9-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7e3f9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="7e3f9-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7e3f9-120">Request headers</span></span>
|<span data-ttu-id="7e3f9-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7e3f9-121">Header</span></span>|<span data-ttu-id="7e3f9-122">値</span><span class="sxs-lookup"><span data-stu-id="7e3f9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e3f9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e3f9-123">Authorization</span></span>|<span data-ttu-id="7e3f9-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7e3f9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e3f9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7e3f9-125">Accept</span></span>|<span data-ttu-id="7e3f9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7e3f9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e3f9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7e3f9-127">Request body</span></span>
<span data-ttu-id="7e3f9-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7e3f9-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7e3f9-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="7e3f9-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7e3f9-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e3f9-130">Property</span></span>|<span data-ttu-id="7e3f9-131">種類</span><span class="sxs-lookup"><span data-stu-id="7e3f9-131">Type</span></span>|<span data-ttu-id="7e3f9-132">説明</span><span class="sxs-lookup"><span data-stu-id="7e3f9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e3f9-133">deviceTag</span><span class="sxs-lookup"><span data-stu-id="7e3f9-133">deviceTag</span></span>|<span data-ttu-id="7e3f9-134">String</span><span class="sxs-lookup"><span data-stu-id="7e3f9-134">String</span></span>|<span data-ttu-id="7e3f9-135">デバイス タグ</span><span class="sxs-lookup"><span data-stu-id="7e3f9-135">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="7e3f9-136">応答</span><span class="sxs-lookup"><span data-stu-id="7e3f9-136">Response</span></span>
<span data-ttu-id="7e3f9-137">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="7e3f9-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7e3f9-138">例</span><span class="sxs-lookup"><span data-stu-id="7e3f9-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e3f9-139">要求</span><span class="sxs-lookup"><span data-stu-id="7e3f9-139">Request</span></span>
<span data-ttu-id="7e3f9-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7e3f9-140">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="7e3f9-141">応答</span><span class="sxs-lookup"><span data-stu-id="7e3f9-141">Response</span></span>
<span data-ttu-id="7e3f9-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7e3f9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



