---
title: OfficeClientConfigurationAssignment を更新します。
description: OfficeClientConfigurationAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d76fd4808c6a9b28151d2487bfb7c6b2afcc7c60
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935193"
---
# <a name="update-officeclientconfigurationassignment"></a><span data-ttu-id="4e061-103">OfficeClientConfigurationAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="4e061-103">Update officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="4e061-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4e061-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e061-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e061-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e061-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4e061-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e061-107">[OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4e061-107">Update the properties of a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4e061-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="4e061-108">Prerequisites</span></span>
<span data-ttu-id="4e061-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4e061-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e061-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4e061-111">Permission type</span></span>|<span data-ttu-id="4e061-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4e061-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e061-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4e061-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e061-114">\* \* TODO: スコープを決定する \* \*</span><span class="sxs-lookup"><span data-stu-id="4e061-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="4e061-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4e061-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e061-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e061-116">Not supported.</span></span>|
|<span data-ttu-id="4e061-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4e061-117">Application</span></span>|<span data-ttu-id="4e061-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e061-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e061-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4e061-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="4e061-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4e061-120">Request headers</span></span>
|<span data-ttu-id="4e061-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4e061-121">Header</span></span>|<span data-ttu-id="4e061-122">値</span><span class="sxs-lookup"><span data-stu-id="4e061-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e061-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e061-123">Authorization</span></span>|<span data-ttu-id="4e061-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4e061-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e061-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4e061-125">Accept</span></span>|<span data-ttu-id="4e061-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e061-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e061-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4e061-127">Request body</span></span>
<span data-ttu-id="4e061-128">要求の本文に[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="4e061-128">In the request body, supply a JSON representation for the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

<span data-ttu-id="4e061-129">[OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="4e061-129">The following table shows the properties that are required when you create the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>

|<span data-ttu-id="4e061-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4e061-130">Property</span></span>|<span data-ttu-id="4e061-131">種類</span><span class="sxs-lookup"><span data-stu-id="4e061-131">Type</span></span>|<span data-ttu-id="4e061-132">説明</span><span class="sxs-lookup"><span data-stu-id="4e061-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e061-133">ID</span><span class="sxs-lookup"><span data-stu-id="4e061-133">id</span></span>|<span data-ttu-id="4e061-134">String</span><span class="sxs-lookup"><span data-stu-id="4e061-134">String</span></span>|<span data-ttu-id="4e061-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4e061-135">Not yet documented</span></span>|
|<span data-ttu-id="4e061-136">ターゲット</span><span class="sxs-lookup"><span data-stu-id="4e061-136">target</span></span>|[<span data-ttu-id="4e061-137">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4e061-137">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="4e061-138">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4e061-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4e061-139">応答</span><span class="sxs-lookup"><span data-stu-id="4e061-139">Response</span></span>
<span data-ttu-id="4e061-140">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="4e061-140">If successful, this method returns a `200 OK` response code and an updated [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e061-141">例</span><span class="sxs-lookup"><span data-stu-id="4e061-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="4e061-142">要求</span><span class="sxs-lookup"><span data-stu-id="4e061-142">Request</span></span>
<span data-ttu-id="4e061-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4e061-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
Content-type: application/json
Content-length: 98

{
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="4e061-144">応答</span><span class="sxs-lookup"><span data-stu-id="4e061-144">Response</span></span>
<span data-ttu-id="4e061-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4e061-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "id": "804730f3-30f3-8047-f330-4780f3304780",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```



