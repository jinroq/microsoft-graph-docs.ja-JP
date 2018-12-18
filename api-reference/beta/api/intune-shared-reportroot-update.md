---
title: reportRoot の更新
description: reportRoot オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 4f3d0e297a9b7d122e9b21afd7555c1af307d2d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349533"
---
# <a name="update-reportroot"></a><span data-ttu-id="07bb8-103">reportRoot の更新</span><span class="sxs-lookup"><span data-stu-id="07bb8-103">Update reportRoot</span></span>

> <span data-ttu-id="07bb8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="07bb8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07bb8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07bb8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07bb8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="07bb8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="07bb8-107">[reportRoot](../resources/intune-shared-reportroot.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="07bb8-107">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="07bb8-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="07bb8-108">Prerequisites</span></span>
<span data-ttu-id="07bb8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="07bb8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07bb8-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="07bb8-111">Permission type</span></span>|<span data-ttu-id="07bb8-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="07bb8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07bb8-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="07bb8-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="07bb8-114">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="07bb8-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="07bb8-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07bb8-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="07bb8-116">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="07bb8-116">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="07bb8-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07bb8-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="07bb8-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="07bb8-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07bb8-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07bb8-119">Not supported.</span></span>|
|<span data-ttu-id="07bb8-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="07bb8-120">Application</span></span>|<span data-ttu-id="07bb8-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07bb8-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07bb8-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="07bb8-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="07bb8-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="07bb8-123">Request headers</span></span>
|<span data-ttu-id="07bb8-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="07bb8-124">Header</span></span>|<span data-ttu-id="07bb8-125">値</span><span class="sxs-lookup"><span data-stu-id="07bb8-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07bb8-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="07bb8-126">Authorization</span></span>|<span data-ttu-id="07bb8-127">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="07bb8-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07bb8-128">Accept</span><span class="sxs-lookup"><span data-stu-id="07bb8-128">Accept</span></span>|<span data-ttu-id="07bb8-129">application/json</span><span class="sxs-lookup"><span data-stu-id="07bb8-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07bb8-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="07bb8-130">Request body</span></span>
<span data-ttu-id="07bb8-131">要求本文で、[reportRoot](../resources/intune-shared-reportroot.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="07bb8-131">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="07bb8-132">次の表に、[reportRoot](../resources/intune-shared-reportroot.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="07bb8-132">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="07bb8-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="07bb8-133">Property</span></span>|<span data-ttu-id="07bb8-134">種類</span><span class="sxs-lookup"><span data-stu-id="07bb8-134">Type</span></span>|<span data-ttu-id="07bb8-135">説明</span><span class="sxs-lookup"><span data-stu-id="07bb8-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07bb8-136">ID</span><span class="sxs-lookup"><span data-stu-id="07bb8-136">id</span></span>|<span data-ttu-id="07bb8-137">String</span><span class="sxs-lookup"><span data-stu-id="07bb8-137">String</span></span>|<span data-ttu-id="07bb8-138">このエンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="07bb8-138">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="07bb8-139">応答</span><span class="sxs-lookup"><span data-stu-id="07bb8-139">Response</span></span>
<span data-ttu-id="07bb8-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [reportRoot](../resources/intune-shared-reportroot.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="07bb8-140">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07bb8-141">例</span><span class="sxs-lookup"><span data-stu-id="07bb8-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="07bb8-142">要求</span><span class="sxs-lookup"><span data-stu-id="07bb8-142">Request</span></span>
<span data-ttu-id="07bb8-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="07bb8-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="07bb8-144">応答</span><span class="sxs-lookup"><span data-stu-id="07bb8-144">Response</span></span>
<span data-ttu-id="07bb8-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="07bb8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```



