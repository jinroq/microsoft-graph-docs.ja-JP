---
title: GroupPolicyPresentationText を作成します。
description: 新しい groupPolicyPresentationText オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4c2bbc1f04ce351afe75a66dd8596f0b52a81e31
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430422"
---
# <a name="create-grouppolicypresentationtext"></a><span data-ttu-id="794a8-103">GroupPolicyPresentationText を作成します。</span><span class="sxs-lookup"><span data-stu-id="794a8-103">Create groupPolicyPresentationText</span></span>

> <span data-ttu-id="794a8-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="794a8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="794a8-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="794a8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="794a8-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="794a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="794a8-107">新しい[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="794a8-107">Create a new [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="794a8-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="794a8-108">Prerequisites</span></span>
<span data-ttu-id="794a8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="794a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="794a8-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="794a8-111">Permission type</span></span>|<span data-ttu-id="794a8-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="794a8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="794a8-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="794a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="794a8-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="794a8-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="794a8-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="794a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="794a8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="794a8-116">Not supported.</span></span>|
|<span data-ttu-id="794a8-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="794a8-117">Application</span></span>|<span data-ttu-id="794a8-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="794a8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="794a8-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="794a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="794a8-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="794a8-120">Request headers</span></span>
|<span data-ttu-id="794a8-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="794a8-121">Header</span></span>|<span data-ttu-id="794a8-122">値</span><span class="sxs-lookup"><span data-stu-id="794a8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="794a8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="794a8-123">Authorization</span></span>|<span data-ttu-id="794a8-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="794a8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="794a8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="794a8-125">Accept</span></span>|<span data-ttu-id="794a8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="794a8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="794a8-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="794a8-127">Request body</span></span>
<span data-ttu-id="794a8-128">要求の本文に groupPolicyPresentationText オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="794a8-128">In the request body, supply a JSON representation for the groupPolicyPresentationText object.</span></span>

<span data-ttu-id="794a8-129">次の表は、groupPolicyPresentationText を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="794a8-129">The following table shows the properties that are required when you create the groupPolicyPresentationText.</span></span>

|<span data-ttu-id="794a8-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="794a8-130">Property</span></span>|<span data-ttu-id="794a8-131">型</span><span class="sxs-lookup"><span data-stu-id="794a8-131">Type</span></span>|<span data-ttu-id="794a8-132">説明</span><span class="sxs-lookup"><span data-stu-id="794a8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="794a8-133">label</span><span class="sxs-lookup"><span data-stu-id="794a8-133">label</span></span>|<span data-ttu-id="794a8-134">String</span><span class="sxs-lookup"><span data-stu-id="794a8-134">String</span></span>|<span data-ttu-id="794a8-135">プレゼンテーションの任意のエンティティのローカライズされたテキスト ラベルです。</span><span class="sxs-lookup"><span data-stu-id="794a8-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="794a8-136">既定値は空です。</span><span class="sxs-lookup"><span data-stu-id="794a8-136">The default value is empty.</span></span> <span data-ttu-id="794a8-137">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="794a8-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="794a8-138">id</span><span class="sxs-lookup"><span data-stu-id="794a8-138">id</span></span>|<span data-ttu-id="794a8-139">String</span><span class="sxs-lookup"><span data-stu-id="794a8-139">String</span></span>|<span data-ttu-id="794a8-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="794a8-140">Key of the entity.</span></span> <span data-ttu-id="794a8-141">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="794a8-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="794a8-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="794a8-142">lastModifiedDateTime</span></span>|<span data-ttu-id="794a8-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="794a8-143">DateTimeOffset</span></span>|<span data-ttu-id="794a8-144">日付と時刻、エンティティが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="794a8-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="794a8-145">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="794a8-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|



## <a name="response"></a><span data-ttu-id="794a8-146">応答</span><span class="sxs-lookup"><span data-stu-id="794a8-146">Response</span></span>
<span data-ttu-id="794a8-147">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="794a8-147">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="794a8-148">例</span><span class="sxs-lookup"><span data-stu-id="794a8-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="794a8-149">要求</span><span class="sxs-lookup"><span data-stu-id="794a8-149">Request</span></span>
<span data-ttu-id="794a8-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="794a8-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="794a8-151">応答</span><span class="sxs-lookup"><span data-stu-id="794a8-151">Response</span></span>
<span data-ttu-id="794a8-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="794a8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 209

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value",
  "id": "bc77d545-d545-bc77-45d5-77bc45d577bc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




