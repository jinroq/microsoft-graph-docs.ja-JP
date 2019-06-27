---
title: Microsoft Graph ツールキットの People コンポーネント
description: '`mgt-people` Web コンポーネントを使用して、ユーザーまたは連絡先のグループを写真またはイニシャルを使用して表示できます。'
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: fcc44262f807d3f10f42e8af8e476975ad262cda
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243062"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="b5749-103">Microsoft Graph ツールキットの People コンポーネント</span><span class="sxs-lookup"><span data-stu-id="b5749-103">People component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="b5749-104">`mgt-people` Web コンポーネントを使用して、ユーザーまたは連絡先のグループを写真またはイニシャルを使用して表示できます。</span><span class="sxs-lookup"><span data-stu-id="b5749-104">You can use the `mgt-people` web component to display a group of people or contacts by using their photos or initials.</span></span> <span data-ttu-id="b5749-105">既定では、サインインしているユーザーの最もよく使用される連絡先が表示されます。</span><span class="sxs-lookup"><span data-stu-id="b5749-105">By default, it will display the most frequent contacts for the signed in user.</span></span>

<span data-ttu-id="b5749-106">このコンポーネントは複数の管理[者](./person.md)を使用していますが、一連のユーザー記述子にバインドできます。</span><span class="sxs-lookup"><span data-stu-id="b5749-106">This component uses multiple [mgt-person](./person.md) controls, but it can be bound to a set of people descriptors.</span></span> <span data-ttu-id="b5749-107">表示するユーザー数がこの`show-max`値を超える場合は、追加の連絡先の数を示す番号が追加されます。</span><span class="sxs-lookup"><span data-stu-id="b5749-107">If there are more people to display than the `show-max` value, a number will be added to indicate the number of additional contacts.</span></span>

## <a name="example"></a><span data-ttu-id="b5749-108">例</span><span class="sxs-lookup"><span data-stu-id="b5749-108">Example</span></span>

[<span data-ttu-id="b5749-109">jsfiddle の例</span><span class="sxs-lookup"><span data-stu-id="b5749-109">jsfiddle example</span></span>](https://jsfiddle.net/metulev/az6pqy2r/)

```html
<mgt-people></mgt-people>
```

![「ユーザー」](./images/mgt-people.png)

## <a name="properties"></a><span data-ttu-id="b5749-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5749-111">Properties</span></span>

<span data-ttu-id="b5749-112">既定では、 `mgt-people`コンポーネントは、頻繁に`/me/people`接続され`personType/class eq 'Person'`たユーザーを表示するために、フィルターを使用してエンドポイントからイベントをフェッチします。</span><span class="sxs-lookup"><span data-stu-id="b5749-112">By default, the `mgt-people` component fetches events from the `/me/people` endpoint with the `personType/class eq 'Person'` filter to display frequently contacted users.</span></span> <span data-ttu-id="b5749-113">この動作を変更するには、いくつかのプロパティを使用できます。</span><span class="sxs-lookup"><span data-stu-id="b5749-113">You can use several properties to change this behavior.</span></span>

| <span data-ttu-id="b5749-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5749-114">Property</span></span> | <span data-ttu-id="b5749-115">属性</span><span class="sxs-lookup"><span data-stu-id="b5749-115">Attribute</span></span> | <span data-ttu-id="b5749-116">説明</span><span class="sxs-lookup"><span data-stu-id="b5749-116">Description</span></span> |
| --- | --- | --- |
| `showMax` | `show-max` | <span data-ttu-id="b5749-117">表示するユーザーの最大数を指定します。</span><span class="sxs-lookup"><span data-stu-id="b5749-117">Indicate the maximum number of people to show.</span></span> <span data-ttu-id="b5749-118">既定値は3です。</span><span class="sxs-lookup"><span data-stu-id="b5749-118">Default value is 3.</span></span> |
| `people` | `people` | <span data-ttu-id="b5749-119">コンポーネントによってレンダリングされたユーザーのリストを取得または設定するユーザーの配列。</span><span class="sxs-lookup"><span data-stu-id="b5749-119">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="b5749-120">このプロパティを使用して、コンポーネントによって読み込まれた人物にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="b5749-120">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="b5749-121">自分のユーザーを読み込むには、この値を設定します。</span><span class="sxs-lookup"><span data-stu-id="b5749-121">Set this value to load your own people.</span></span> |

<span data-ttu-id="b5749-122">次の例では、表示するユーザーの最大数を設定します。</span><span class="sxs-lookup"><span data-stu-id="b5749-122">The following example sets the maximum number of people to show.</span></span>

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a><span data-ttu-id="b5749-123">CSS カスタムプロパティ</span><span class="sxs-lookup"><span data-stu-id="b5749-123">CSS custom properties</span></span>

<span data-ttu-id="b5749-124">コンポーネント`mgt-people`は、次の CSS カスタムプロパティを定義します。</span><span class="sxs-lookup"><span data-stu-id="b5749-124">The `mgt-people` component defines the following CSS custom properties.</span></span>

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
}
```

## <a name="templates"></a><span data-ttu-id="b5749-125">テンプレート</span><span class="sxs-lookup"><span data-stu-id="b5749-125">Templates</span></span>

<span data-ttu-id="b5749-126">は`mgt-people` 、コンポーネントの特定の部分を置き換えるために使用できるいくつかの[テンプレート](../templates.md)をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="b5749-126">The `mgt-people` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="b5749-127">テンプレートを指定するには、 `<template>`コンポーネント内に要素を含め、 `data-type`値を次のいずれかに設定します。</span><span class="sxs-lookup"><span data-stu-id="b5749-127">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="b5749-128">データ型</span><span class="sxs-lookup"><span data-stu-id="b5749-128">Data type</span></span> | <span data-ttu-id="b5749-129">データコンテキスト</span><span class="sxs-lookup"><span data-stu-id="b5749-129">Data context</span></span> | <span data-ttu-id="b5749-130">説明</span><span class="sxs-lookup"><span data-stu-id="b5749-130">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="b5749-131">`people`: person オブジェクトのリスト</span><span class="sxs-lookup"><span data-stu-id="b5749-131">`people`: list of person objects</span></span> | <span data-ttu-id="b5749-132">既定のテンプレートでは、コンポーネント全体が独自のものに置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="b5749-132">The default template replaces the entire component with your own.</span></span> |
| `person` | <span data-ttu-id="b5749-133">`person`: person オブジェクト</span><span class="sxs-lookup"><span data-stu-id="b5749-133">`person`: person object</span></span> | <span data-ttu-id="b5749-134">各ユーザーのレンダリングに使用するテンプレート。</span><span class="sxs-lookup"><span data-stu-id="b5749-134">The template used to render each person.</span></span> |
| `overflow` | <span data-ttu-id="b5749-135">`people`: person オブジェクトのリスト</span><span class="sxs-lookup"><span data-stu-id="b5749-135">`people`: list of person objects</span></span> <br> <span data-ttu-id="b5749-136">`max`: 表示されているユーザーの数</span><span class="sxs-lookup"><span data-stu-id="b5749-136">`max`: number of shown people</span></span> <br> <span data-ttu-id="b5749-137">`extra`: 特別なユーザーの数</span><span class="sxs-lookup"><span data-stu-id="b5749-137">`extra`: number of extra people</span></span> | <span data-ttu-id="b5749-138">ユーザーの一覧の右側に最大数を超える番号をレンダリングするために使用されるテンプレート。</span><span class="sxs-lookup"><span data-stu-id="b5749-138">The template used to render the number beyond the max to the right of the list of people.</span></span> |
| `no-data` | <span data-ttu-id="b5749-139">データコンテキストが渡されない</span><span class="sxs-lookup"><span data-stu-id="b5749-139">No data context is passed</span></span> | <span data-ttu-id="b5749-140">ユーザーが使用できない場合に使用するテンプレート。</span><span class="sxs-lookup"><span data-stu-id="b5749-140">The template used when no people are available.</span></span> |

<span data-ttu-id="b5749-141">次の例は、テンプレートの`person`使用方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="b5749-141">The following examples shows how to use the `person` template.</span></span>

```html
<mgt-people>
  <template>
    <ul><li data-for="person in people">
      <mgt-person person-query="{{ person.userPrincipalName }}"></mgt-person>
      <h3>{{ person.displayName }}</h3>
      <p>{{ person.jobTitle }}</p>
      <p>{{ person.department }}</p>
    </li></ul>
  </template>
</mgt-people>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="b5749-142">Microsoft Graph のアクセス許可</span><span class="sxs-lookup"><span data-stu-id="b5749-142">Microsoft Graph permissions</span></span>

<span data-ttu-id="b5749-143">このコンポーネントは、次の Microsoft Graph Api とアクセス許可を使用します。</span><span class="sxs-lookup"><span data-stu-id="b5749-143">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="b5749-144">リソース</span><span class="sxs-lookup"><span data-stu-id="b5749-144">Resource</span></span> | <span data-ttu-id="b5749-145">アクセス許可/スコープ</span><span class="sxs-lookup"><span data-stu-id="b5749-145">Permission/scope</span></span> |
| - | - |
| [<span data-ttu-id="b5749-146">/me/ユーザー</span><span class="sxs-lookup"><span data-stu-id="b5749-146">/me/people</span></span>](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0) | `People.Read` |

## <a name="authentication"></a><span data-ttu-id="b5749-147">認証</span><span class="sxs-lookup"><span data-stu-id="b5749-147">Authentication</span></span>

<span data-ttu-id="b5749-148">このコントロールは、[認証のドキュメント](./../providers.md)で説明されているグローバル認証プロバイダを使用します。</span><span class="sxs-lookup"><span data-stu-id="b5749-148">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
