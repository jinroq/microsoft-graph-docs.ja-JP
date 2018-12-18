---
title: Delete androidCustomConfiguration
description: androidCustomConfiguration を削除します。
author: tfitzmac
ms.openlocfilehash: 06af1113f18dca40b39e1826db5a26af0f317685
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327861"
---
# <a name="delete-androidcustomconfiguration"></a><span data-ttu-id="b3400-103">Delete androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="b3400-103">Delete androidCustomConfiguration</span></span>

> <span data-ttu-id="b3400-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b3400-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3400-105">[androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="b3400-105">Deletes a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b3400-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="b3400-106">Prerequisites</span></span>
<span data-ttu-id="b3400-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b3400-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3400-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b3400-109">Permission type</span></span>|<span data-ttu-id="b3400-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b3400-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3400-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b3400-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b3400-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3400-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b3400-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b3400-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3400-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3400-114">Not supported.</span></span>|
|<span data-ttu-id="b3400-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b3400-115">Application</span></span>|<span data-ttu-id="b3400-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3400-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3400-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b3400-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b3400-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b3400-118">Request headers</span></span>
|<span data-ttu-id="b3400-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b3400-119">Header</span></span>|<span data-ttu-id="b3400-120">値</span><span class="sxs-lookup"><span data-stu-id="b3400-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3400-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3400-121">Authorization</span></span>|<span data-ttu-id="b3400-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b3400-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3400-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b3400-123">Accept</span></span>|<span data-ttu-id="b3400-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b3400-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3400-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b3400-125">Request body</span></span>
<span data-ttu-id="b3400-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b3400-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3400-127">応答</span><span class="sxs-lookup"><span data-stu-id="b3400-127">Response</span></span>
<span data-ttu-id="b3400-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="b3400-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b3400-129">例</span><span class="sxs-lookup"><span data-stu-id="b3400-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="b3400-130">要求</span><span class="sxs-lookup"><span data-stu-id="b3400-130">Request</span></span>
<span data-ttu-id="b3400-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b3400-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="b3400-132">応答</span><span class="sxs-lookup"><span data-stu-id="b3400-132">Response</span></span>
<span data-ttu-id="b3400-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b3400-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



