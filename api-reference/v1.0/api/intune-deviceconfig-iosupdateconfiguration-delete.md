---
title: iosUpdateConfiguration の削除
description: iosUpdateConfiguration を削除します。
author: tfitzmac
ms.openlocfilehash: 08d7d0a8bee77165878f185c2136a36dec3ef0f3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343709"
---
# <a name="delete-iosupdateconfiguration"></a><span data-ttu-id="f3e8c-103">iosUpdateConfiguration の削除</span><span class="sxs-lookup"><span data-stu-id="f3e8c-103">Delete iosUpdateConfiguration</span></span>

> <span data-ttu-id="f3e8c-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f3e8c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3e8c-105">[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="f3e8c-105">Deletes a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f3e8c-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="f3e8c-106">Prerequisites</span></span>
<span data-ttu-id="f3e8c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3e8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3e8c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f3e8c-109">Permission type</span></span>|<span data-ttu-id="f3e8c-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f3e8c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3e8c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f3e8c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f3e8c-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3e8c-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f3e8c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f3e8c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3e8c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3e8c-114">Not supported.</span></span>|
|<span data-ttu-id="f3e8c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f3e8c-115">Application</span></span>|<span data-ttu-id="f3e8c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3e8c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3e8c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f3e8c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f3e8c-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3e8c-118">Request headers</span></span>
|<span data-ttu-id="f3e8c-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3e8c-119">Header</span></span>|<span data-ttu-id="f3e8c-120">値</span><span class="sxs-lookup"><span data-stu-id="f3e8c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3e8c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3e8c-121">Authorization</span></span>|<span data-ttu-id="f3e8c-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f3e8c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3e8c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f3e8c-123">Accept</span></span>|<span data-ttu-id="f3e8c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f3e8c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3e8c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f3e8c-125">Request body</span></span>
<span data-ttu-id="f3e8c-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f3e8c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3e8c-127">応答</span><span class="sxs-lookup"><span data-stu-id="f3e8c-127">Response</span></span>
<span data-ttu-id="f3e8c-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="f3e8c-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f3e8c-129">例</span><span class="sxs-lookup"><span data-stu-id="f3e8c-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="f3e8c-130">要求</span><span class="sxs-lookup"><span data-stu-id="f3e8c-130">Request</span></span>
<span data-ttu-id="f3e8c-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f3e8c-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="f3e8c-132">応答</span><span class="sxs-lookup"><span data-stu-id="f3e8c-132">Response</span></span>
<span data-ttu-id="f3e8c-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f3e8c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



