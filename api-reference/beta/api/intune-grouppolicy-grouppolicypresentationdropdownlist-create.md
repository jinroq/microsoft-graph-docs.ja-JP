---
title: GroupPolicyPresentationDropdownList の作成
description: 新しい groupPolicyPresentationDropdownList オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 982ba88b60df569ec58aba15de74e6d87f9231db
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964795"
---
# <a name="create-grouppolicypresentationdropdownlist"></a><span data-ttu-id="bdc5c-103">GroupPolicyPresentationDropdownList の作成</span><span class="sxs-lookup"><span data-stu-id="bdc5c-103">Create groupPolicyPresentationDropdownList</span></span>

> <span data-ttu-id="bdc5c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bdc5c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bdc5c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bdc5c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdc5c-106">新しい[Grouppolicypresentationdropdownlist](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="bdc5c-106">Create a new [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bdc5c-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="bdc5c-107">Prerequisites</span></span>
<span data-ttu-id="bdc5c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bdc5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdc5c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bdc5c-110">Permission type</span></span>|<span data-ttu-id="bdc5c-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bdc5c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bdc5c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bdc5c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bdc5c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdc5c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bdc5c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bdc5c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bdc5c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bdc5c-115">Not supported.</span></span>|
|<span data-ttu-id="bdc5c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bdc5c-116">Application</span></span>|<span data-ttu-id="bdc5c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bdc5c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bdc5c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bdc5c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="bdc5c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bdc5c-119">Request headers</span></span>
|<span data-ttu-id="bdc5c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bdc5c-120">Header</span></span>|<span data-ttu-id="bdc5c-121">値</span><span class="sxs-lookup"><span data-stu-id="bdc5c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bdc5c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdc5c-122">Authorization</span></span>|<span data-ttu-id="bdc5c-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="bdc5c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bdc5c-124">承諾</span><span class="sxs-lookup"><span data-stu-id="bdc5c-124">Accept</span></span>|<span data-ttu-id="bdc5c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bdc5c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdc5c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="bdc5c-126">Request body</span></span>
<span data-ttu-id="bdc5c-127">要求本文で、groupPolicyPresentationDropdownList オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="bdc5c-127">In the request body, supply a JSON representation for the groupPolicyPresentationDropdownList object.</span></span>

<span data-ttu-id="bdc5c-128">次の表に、groupPolicyPresentationDropdownList の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="bdc5c-128">The following table shows the properties that are required when you create the groupPolicyPresentationDropdownList.</span></span>

|<span data-ttu-id="bdc5c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bdc5c-129">Property</span></span>|<span data-ttu-id="bdc5c-130">型</span><span class="sxs-lookup"><span data-stu-id="bdc5c-130">Type</span></span>|<span data-ttu-id="bdc5c-131">説明</span><span class="sxs-lookup"><span data-stu-id="bdc5c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdc5c-132">label</span><span class="sxs-lookup"><span data-stu-id="bdc5c-132">label</span></span>|<span data-ttu-id="bdc5c-133">String</span><span class="sxs-lookup"><span data-stu-id="bdc5c-133">String</span></span>|<span data-ttu-id="bdc5c-134">任意のプレゼンテーションエンティティのローカライズされたテキストラベル。</span><span class="sxs-lookup"><span data-stu-id="bdc5c-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="bdc5c-135">既定値は空白です。</span><span class="sxs-lookup"><span data-stu-id="bdc5c-135">The default value is empty.</span></span> <span data-ttu-id="bdc5c-136">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="bdc5c-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="bdc5c-137">id</span><span class="sxs-lookup"><span data-stu-id="bdc5c-137">id</span></span>|<span data-ttu-id="bdc5c-138">String</span><span class="sxs-lookup"><span data-stu-id="bdc5c-138">String</span></span>|<span data-ttu-id="bdc5c-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="bdc5c-139">Key of the entity.</span></span> <span data-ttu-id="bdc5c-140">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="bdc5c-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="bdc5c-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bdc5c-141">lastModifiedDateTime</span></span>|<span data-ttu-id="bdc5c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdc5c-142">DateTimeOffset</span></span>|<span data-ttu-id="bdc5c-143">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="bdc5c-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="bdc5c-144">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="bdc5c-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="bdc5c-145">defaultItem</span><span class="sxs-lookup"><span data-stu-id="bdc5c-145">defaultItem</span></span>|[<span data-ttu-id="bdc5c-146">groupPolicyPresentationDropdownListItem</span><span class="sxs-lookup"><span data-stu-id="bdc5c-146">groupPolicyPresentationDropdownListItem</span></span>](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|<span data-ttu-id="bdc5c-147">アイテムのリストの既定の選択を示すローカライズされた文字列値。</span><span class="sxs-lookup"><span data-stu-id="bdc5c-147">Localized string value identifying the default choice of the list of items.</span></span>|
|<span data-ttu-id="bdc5c-148">items</span><span class="sxs-lookup"><span data-stu-id="bdc5c-148">items</span></span>|<span data-ttu-id="bdc5c-149">[Grouppolicypresentationdropdownlistitem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bdc5c-149">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) collection</span></span>|<span data-ttu-id="bdc5c-150">ローカライズされた表示名とそれに関連する値のセットを表します。</span><span class="sxs-lookup"><span data-stu-id="bdc5c-150">Represents a set of localized display names and their associated values.</span></span>|
|<span data-ttu-id="bdc5c-151">必須</span><span class="sxs-lookup"><span data-stu-id="bdc5c-151">required</span></span>|<span data-ttu-id="bdc5c-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="bdc5c-152">Boolean</span></span>|<span data-ttu-id="bdc5c-153">[パラメーター] ボックスに値を入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="bdc5c-153">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="bdc5c-154">既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="bdc5c-154">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="bdc5c-155">応答</span><span class="sxs-lookup"><span data-stu-id="bdc5c-155">Response</span></span>
<span data-ttu-id="bdc5c-156">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Grouppolicypresentationdropdownlist](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bdc5c-156">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdc5c-157">例</span><span class="sxs-lookup"><span data-stu-id="bdc5c-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="bdc5c-158">要求</span><span class="sxs-lookup"><span data-stu-id="bdc5c-158">Request</span></span>
<span data-ttu-id="bdc5c-159">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bdc5c-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 489

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDropdownList",
  "label": "Label value",
  "defaultItem": {
    "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
    "displayName": "Display Name value",
    "value": "Value value"
  },
  "items": [
    {
      "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
      "displayName": "Display Name value",
      "value": "Value value"
    }
  ],
  "required": true
}
```

### <a name="response"></a><span data-ttu-id="bdc5c-160">応答</span><span class="sxs-lookup"><span data-stu-id="bdc5c-160">Response</span></span>
<span data-ttu-id="bdc5c-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bdc5c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 602

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDropdownList",
  "label": "Label value",
  "id": "ba3ff7c9-f7c9-ba3f-c9f7-3fbac9f73fba",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultItem": {
    "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
    "displayName": "Display Name value",
    "value": "Value value"
  },
  "items": [
    {
      "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
      "displayName": "Display Name value",
      "value": "Value value"
    }
  ],
  "required": true
}
```





