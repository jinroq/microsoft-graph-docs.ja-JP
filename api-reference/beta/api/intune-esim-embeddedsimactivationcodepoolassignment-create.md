---
title: EmbeddedSIMActivationCodePoolAssignment を作成します。
description: 新しい embeddedSIMActivationCodePoolAssignment オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d42ab3e6444a98019e4e54fdd3e5f6719dfa66e2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409126"
---
# <a name="create-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="2bbff-103">EmbeddedSIMActivationCodePoolAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="2bbff-103">Create embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="2bbff-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2bbff-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2bbff-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2bbff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2bbff-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2bbff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bbff-107">新しい[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2bbff-107">Create a new [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2bbff-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="2bbff-108">Prerequisites</span></span>
<span data-ttu-id="2bbff-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2bbff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2bbff-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2bbff-111">Permission type</span></span>|<span data-ttu-id="2bbff-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2bbff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bbff-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2bbff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2bbff-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bbff-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2bbff-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2bbff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bbff-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2bbff-116">Not supported.</span></span>|
|<span data-ttu-id="2bbff-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2bbff-117">Application</span></span>|<span data-ttu-id="2bbff-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2bbff-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bbff-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2bbff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="2bbff-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2bbff-120">Request headers</span></span>
|<span data-ttu-id="2bbff-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2bbff-121">Header</span></span>|<span data-ttu-id="2bbff-122">値</span><span class="sxs-lookup"><span data-stu-id="2bbff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bbff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bbff-123">Authorization</span></span>|<span data-ttu-id="2bbff-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2bbff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bbff-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2bbff-125">Accept</span></span>|<span data-ttu-id="2bbff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2bbff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bbff-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2bbff-127">Request body</span></span>
<span data-ttu-id="2bbff-128">要求の本文に embeddedSIMActivationCodePoolAssignment オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="2bbff-128">In the request body, supply a JSON representation for the embeddedSIMActivationCodePoolAssignment object.</span></span>

<span data-ttu-id="2bbff-129">次の表は、embeddedSIMActivationCodePoolAssignment を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2bbff-129">The following table shows the properties that are required when you create the embeddedSIMActivationCodePoolAssignment.</span></span>

|<span data-ttu-id="2bbff-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2bbff-130">Property</span></span>|<span data-ttu-id="2bbff-131">型</span><span class="sxs-lookup"><span data-stu-id="2bbff-131">Type</span></span>|<span data-ttu-id="2bbff-132">説明</span><span class="sxs-lookup"><span data-stu-id="2bbff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bbff-133">id</span><span class="sxs-lookup"><span data-stu-id="2bbff-133">id</span></span>|<span data-ttu-id="2bbff-134">String</span><span class="sxs-lookup"><span data-stu-id="2bbff-134">String</span></span>|<span data-ttu-id="2bbff-135">埋め込み SIM アクティベーション コードのプール割り当ての一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="2bbff-135">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="2bbff-136">システムでは、作成時に割り当てられた値が生成されます。</span><span class="sxs-lookup"><span data-stu-id="2bbff-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="2bbff-137">target</span><span class="sxs-lookup"><span data-stu-id="2bbff-137">target</span></span>|[<span data-ttu-id="2bbff-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2bbff-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2bbff-139">SIM のアクティブ化コードの埋め込み、プールの対象となるグループの種類。</span><span class="sxs-lookup"><span data-stu-id="2bbff-139">The type of groups targeted by the embedded SIM activation code pool.</span></span>|



## <a name="response"></a><span data-ttu-id="2bbff-140">応答</span><span class="sxs-lookup"><span data-stu-id="2bbff-140">Response</span></span>
<span data-ttu-id="2bbff-141">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="2bbff-141">If successful, this method returns a `201 Created` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bbff-142">例</span><span class="sxs-lookup"><span data-stu-id="2bbff-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="2bbff-143">要求</span><span class="sxs-lookup"><span data-stu-id="2bbff-143">Request</span></span>
<span data-ttu-id="2bbff-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2bbff-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="2bbff-145">応答</span><span class="sxs-lookup"><span data-stu-id="2bbff-145">Response</span></span>
<span data-ttu-id="2bbff-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2bbff-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




