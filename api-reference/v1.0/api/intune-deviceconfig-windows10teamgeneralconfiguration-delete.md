---
title: windows10TeamGeneralConfiguration の削除
description: windows10TeamGeneralConfiguration を削除します。
ms.openlocfilehash: f1e99cc8c45ea5bfcddb97712f354daa14f8bba7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023350"
---
# <a name="delete-windows10teamgeneralconfiguration"></a><span data-ttu-id="b4d12-103">windows10TeamGeneralConfiguration の削除</span><span class="sxs-lookup"><span data-stu-id="b4d12-103">Delete windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="b4d12-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b4d12-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4d12-105">[windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="b4d12-105">Deletes a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4d12-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="b4d12-106">Prerequisites</span></span>
<span data-ttu-id="b4d12-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b4d12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4d12-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b4d12-109">Permission type</span></span>|<span data-ttu-id="b4d12-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b4d12-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4d12-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b4d12-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b4d12-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4d12-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b4d12-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b4d12-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4d12-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4d12-114">Not supported.</span></span>|
|<span data-ttu-id="b4d12-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b4d12-115">Application</span></span>|<span data-ttu-id="b4d12-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4d12-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4d12-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b4d12-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b4d12-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b4d12-118">Request headers</span></span>
|<span data-ttu-id="b4d12-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b4d12-119">Header</span></span>|<span data-ttu-id="b4d12-120">値</span><span class="sxs-lookup"><span data-stu-id="b4d12-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4d12-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4d12-121">Authorization</span></span>|<span data-ttu-id="b4d12-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b4d12-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4d12-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b4d12-123">Accept</span></span>|<span data-ttu-id="b4d12-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b4d12-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4d12-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b4d12-125">Request body</span></span>
<span data-ttu-id="b4d12-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b4d12-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4d12-127">応答</span><span class="sxs-lookup"><span data-stu-id="b4d12-127">Response</span></span>
<span data-ttu-id="b4d12-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="b4d12-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b4d12-129">例</span><span class="sxs-lookup"><span data-stu-id="b4d12-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="b4d12-130">要求</span><span class="sxs-lookup"><span data-stu-id="b4d12-130">Request</span></span>
<span data-ttu-id="b4d12-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b4d12-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="b4d12-132">応答</span><span class="sxs-lookup"><span data-stu-id="b4d12-132">Response</span></span>
<span data-ttu-id="b4d12-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b4d12-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```


