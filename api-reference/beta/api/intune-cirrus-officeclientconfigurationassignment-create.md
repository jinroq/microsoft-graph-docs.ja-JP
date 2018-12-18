---
title: OfficeClientConfigurationAssignment を作成します。
description: ターゲット グループを既存のポリシーに追加します。
author: tfitzmac
ms.openlocfilehash: 850f82f005f46e15a598dd0e08043cca66ffe6bf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324837"
---
# <a name="create-officeclientconfigurationassignment"></a><span data-ttu-id="d8ca6-103">OfficeClientConfigurationAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="d8ca6-103">Create officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="d8ca6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d8ca6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8ca6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8ca6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8ca6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d8ca6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8ca6-107">ターゲット グループを既存のポリシーに追加します。</span><span class="sxs-lookup"><span data-stu-id="d8ca6-107">Add a target group to an existing policy.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d8ca6-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="d8ca6-108">Prerequisites</span></span>
<span data-ttu-id="d8ca6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d8ca6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8ca6-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d8ca6-111">Permission type</span></span>|<span data-ttu-id="d8ca6-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d8ca6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8ca6-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d8ca6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d8ca6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8ca6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d8ca6-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d8ca6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8ca6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8ca6-116">Not supported.</span></span>|
|<span data-ttu-id="d8ca6-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d8ca6-117">Application</span></span>|<span data-ttu-id="d8ca6-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8ca6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8ca6-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d8ca6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{key}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="d8ca6-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d8ca6-120">Request headers</span></span>
|<span data-ttu-id="d8ca6-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d8ca6-121">Header</span></span>|<span data-ttu-id="d8ca6-122">値</span><span class="sxs-lookup"><span data-stu-id="d8ca6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8ca6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8ca6-123">Authorization</span></span>|<span data-ttu-id="d8ca6-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d8ca6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8ca6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d8ca6-125">Accept</span></span>|<span data-ttu-id="d8ca6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d8ca6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8ca6-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d8ca6-127">Request body</span></span>
<span data-ttu-id="d8ca6-128">要求の本文に officeClientConfigurationAssignment オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="d8ca6-128">In the request body, supply a JSON representation for the officeClientConfigurationAssignment object.</span></span>

<span data-ttu-id="d8ca6-129">次の表は、officeClientConfigurationAssignment を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d8ca6-129">The following table shows the properties that are required when you create the officeClientConfigurationAssignment.</span></span>

|<span data-ttu-id="d8ca6-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d8ca6-130">Property</span></span>|<span data-ttu-id="d8ca6-131">種類</span><span class="sxs-lookup"><span data-stu-id="d8ca6-131">Type</span></span>|<span data-ttu-id="d8ca6-132">説明</span><span class="sxs-lookup"><span data-stu-id="d8ca6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8ca6-133">ID</span><span class="sxs-lookup"><span data-stu-id="d8ca6-133">id</span></span>|<span data-ttu-id="d8ca6-134">String</span><span class="sxs-lookup"><span data-stu-id="d8ca6-134">String</span></span>|<span data-ttu-id="d8ca6-135">OfficeConfigurationAssignment の id です。</span><span class="sxs-lookup"><span data-stu-id="d8ca6-135">Id of the OfficeConfigurationAssignment.</span></span>|
|<span data-ttu-id="d8ca6-136">ターゲット</span><span class="sxs-lookup"><span data-stu-id="d8ca6-136">target</span></span>|[<span data-ttu-id="d8ca6-137">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d8ca6-137">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="d8ca6-138">Admin によって定義されているターゲットの割り当て</span><span class="sxs-lookup"><span data-stu-id="d8ca6-138">The target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="d8ca6-139">応答</span><span class="sxs-lookup"><span data-stu-id="d8ca6-139">Response</span></span>
<span data-ttu-id="d8ca6-140">かどうかは成功すると、このメソッドが返されます、`200 Created`応答コードおよび応答の本文に[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="d8ca6-140">If successful, this method returns a `200 Created` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8ca6-141">例</span><span class="sxs-lookup"><span data-stu-id="d8ca6-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="d8ca6-142">要求</span><span class="sxs-lookup"><span data-stu-id="d8ca6-142">Request</span></span>
<span data-ttu-id="d8ca6-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d8ca6-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="d8ca6-144">応答</span><span class="sxs-lookup"><span data-stu-id="d8ca6-144">Response</span></span>
<span data-ttu-id="d8ca6-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d8ca6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



