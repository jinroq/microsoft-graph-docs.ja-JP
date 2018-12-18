---
title: iosLobApp の削除
description: iosLobApp を削除します。
author: tfitzmac
ms.openlocfilehash: 71c7932ad118656674689592864ed12d7705da32
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323248"
---
# <a name="delete-ioslobapp"></a><span data-ttu-id="f9bcd-103">iosLobApp の削除</span><span class="sxs-lookup"><span data-stu-id="f9bcd-103">Delete iosLobApp</span></span>

> <span data-ttu-id="f9bcd-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f9bcd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f9bcd-105">[iosLobApp](../resources/intune-apps-ioslobapp.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="f9bcd-105">Deletes a [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f9bcd-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="f9bcd-106">Prerequisites</span></span>
<span data-ttu-id="f9bcd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f9bcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9bcd-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f9bcd-109">Permission type</span></span>|<span data-ttu-id="f9bcd-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f9bcd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9bcd-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f9bcd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f9bcd-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9bcd-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f9bcd-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f9bcd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9bcd-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9bcd-114">Not supported.</span></span>|
|<span data-ttu-id="f9bcd-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f9bcd-115">Application</span></span>|<span data-ttu-id="f9bcd-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9bcd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9bcd-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f9bcd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="f9bcd-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f9bcd-118">Request headers</span></span>
|<span data-ttu-id="f9bcd-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f9bcd-119">Header</span></span>|<span data-ttu-id="f9bcd-120">値</span><span class="sxs-lookup"><span data-stu-id="f9bcd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9bcd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9bcd-121">Authorization</span></span>|<span data-ttu-id="f9bcd-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f9bcd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9bcd-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f9bcd-123">Accept</span></span>|<span data-ttu-id="f9bcd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f9bcd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9bcd-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f9bcd-125">Request body</span></span>
<span data-ttu-id="f9bcd-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f9bcd-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9bcd-127">応答</span><span class="sxs-lookup"><span data-stu-id="f9bcd-127">Response</span></span>
<span data-ttu-id="f9bcd-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="f9bcd-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f9bcd-129">例</span><span class="sxs-lookup"><span data-stu-id="f9bcd-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="f9bcd-130">要求</span><span class="sxs-lookup"><span data-stu-id="f9bcd-130">Request</span></span>
<span data-ttu-id="f9bcd-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f9bcd-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="f9bcd-132">応答</span><span class="sxs-lookup"><span data-stu-id="f9bcd-132">Response</span></span>
<span data-ttu-id="f9bcd-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f9bcd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



